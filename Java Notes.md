- Convert character to index (We are assuming that all character are lowercase alphabets in the range a-z)
 <pre markdown="1"> int idx = ch - 'a'</pre>
- Removing BoilerPlate code for map
<pre markdown="1"> Map&lt;Integer,List&lt;Integer>> map = new HashMap<>();
List<Integer> list = map.getOrDefault(k, new ArrayList<>());
list.add(value);
map.put(k, list);
</pre>   Replace with

<pre markdown="1"> map.computeIfAfsent(k, key -> new ArrayList<>()).add(value);
</pre>
