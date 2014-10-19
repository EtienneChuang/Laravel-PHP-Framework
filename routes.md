<h3>Test routes</h3>
Edit <i>routes.php</i> which is under dir <i>app</i><br/>
Type the following code in and the save : <br>
<pre><code>
  Route::get('/users', function()
  {
      return 'Hello Users!';
  });
</code></pre>
Type an URL on the broswer, I tested on localhost, so the URL is gonna be <i>127.0.01/Laravel-master/<b>public</b>/users</i>.<br/>
And and a page with 'Hello Users' will be given.<br>
<b>IMPORTANT</b> : <i>public</i> should come after the domain name(i.e 127.0.01/Laravel-master in this example), or the result will be 404 not found.
