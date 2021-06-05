public String MGCheckKey(JSONObject MGGetObject, String MGGetKey, String MGSetDefault) throws JSONException {

		String setReturn = "-";
        
			if (MGGetObject.has(MGGetKey)) {
        
				String setKey = MGGetObject.getString(MGGetKey);
            
				if (setKey.equalsIgnoreCase("") || setKey.isEmpty() || setKey == null) {
            
					setReturn = MGSetDefault;
                
				} else {
            
					setReturn = setKey;
                
				}
            
			} else {
        
				setReturn = MGSetDefault;
            
			}
        
			return setReturn;
        
}
