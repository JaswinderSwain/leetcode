<h2><a href="https://leetcode.com/problems/insert-delete-getrandom-o1/description/?envType=daily-question&envId=2024-01-16">380: Insert Delete GetRandom O(1)</a></h2>
<h3>Medium</h3>

<p>Implement the RandomizedSet class:</p>

<code>RandomizedSet()</code> Initializes the RandomizedSet object.
<code>bool insert(int val)</code> Inserts an item val into the set if not present. Returns true if the item was not present, false otherwise.
<code>bool remove(int val)</code> Removes an item val from the set if present. Returns true if the item was present, false otherwise.
<code>int getRandom()</code> Returns a random element from the current set of elements (it's guaranteed that at least one element exists when this method is called). Each element must have the same probability of being returned.
You must implement the functions of the class such that each function works in average O(1) time complexity.

<p>&nbsp;</p>
<p><strong class="example">Example 1:</strong></p>

<p><strong>Input</strong></p>
<pre>
["RandomizedSet", "insert", "remove", "insert", "getRandom", "remove", "insert", "getRandom"]
[[], [1], [2], [2], [], [1], [2], []]
</pre>

<p><strong>Output</strong></p>
<pre>
[null, true, false, true, 2, true, false, 2]
</pre>

<p><strong>Explanation</strong></p>
<pre>
RandomizedSet randomizedSet = new RandomizedSet();
randomizedSet.insert(1); // Inserts 1 to the set. Returns true as 1 was inserted successfully.
randomizedSet.remove(2); // Returns false as 2 does not exist in the set.
randomizedSet.insert(2); // Inserts 2 to the set, returns true. Set now contains [1,2].
randomizedSet.getRandom(); // getRandom() should return either 1 or 2 randomly.
randomizedSet.remove(1); // Removes 1 from the set, returns true. Set now contains [2].
randomizedSet.insert(2); // 2 was already in the set, so return false.
randomizedSet.getRandom(); // Since 2 is the only number in the set, getRandom() will always return 2.
</pre>

<p><strong>Constraints:</strong></p>

<ul>
  <li>-231 <= val <= 231 - 1</li>
  <li>At most 2 * 105 calls will be made to insert, remove, and getRandom.</li>
  <li>There will be at least one element in the data structure when getRandom is called.</li>
</ul>
