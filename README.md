# SecureRestClient
A stateful and cookie authentification RestClient wrapping Spring RestTemplate

Usage:
		SecureRestClient client = new SecureRestClient();
		client.setHost("ivr.africasys.com");
		client.setPort("80");
		client.setApiPath("");
		client.setApplicationPath("afrivox");
		client.login("user", "password");
		Integer callsNumber = client.template().getForObject(client.apiUrl("callsnumber"), Integer.class);
