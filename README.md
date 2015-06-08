# ClientMedia
JavaClient for the Mediaserver using org.apache.httpcomponents.

Posting : Where myJSON is a  String with key:value,key:value

StringEntity entity = new StringEntity(myJSON, ContentType.APPLICATION_JSON);
String url = "http://127.0.0.1:8080/MediaServerResteasy/media";
HttpPost post = new HttpPost(url);
post.setEntity(entity);
response = client.execute(post);

