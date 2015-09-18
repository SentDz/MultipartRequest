# MultipartRequest
a volley custom request to support file upload


<p>How to use:</p>
<pre><code>
MultipartRequestParams params = new MultipartRequestParams();
params.put("userName",username);
params.put("myfiles",files);
getVolleyRequestQueue().add(new MultipartRequest(Request.Method.POST, params, URL, new Response.Listener<String>() {
            @Override
            public void onResponse(String response) {
                //TODO
            }
        }, new Response.ErrorListener() {
            @Override
            public void onErrorResponse(VolleyError error) {
                //TODO
            }
        }));

</code></pre>

