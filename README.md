# MGCheckJsonKey
Check if a key exists and if it is empty or null

In some situations we have to apply the well known expression "trust does not exclude control".

It is in this context that I provide this small function that allows you to control the existence of a key in a JSONObject. But also control if the key is Null, Empty or =" ".

To use this function you must give it a JSONObject, a key and a default value.

public String MGCheckKey(JSONObject MGGetObject, String MGGetKey, String MGSetDefault) throws JSONException

Example: 

JSONObject json = new JSONObject(params);
JSONArray jsonarray = json.getJSONArray("MY_ARRAY");

	for (int i = 0; i < jsonarray.length(); i++) {
		JSONObject jsonObj = jsonarray.getJSONObject(i);

		String myValue1 = MGCheckKey(jsonObj, "key1", "Default value #1");
		String myValue2 = MGCheckKey(jsonObj, "key2", "Default value 2");

	}
