<h3>Test routes</h3>
Edit <i>routes.php</i> which is under dir <i>app</i><br/>
Type the following code in and the save : <br>
<pre>
  Route::get('/users', function()
  {
      return 'Hello Users!';
  });
</pre>
Type an URL on the broswer, I tested on localhost, so the URL is gonna be <i>127.0.01/Laravel-master/<b>public</b>/users</i>.<br/>
And and a page with 'Hello Users' will be given.<br>
<b>IMPORTANT</b> : <i>public</i> should come after the domain name(i.e 127.0.0.1/Laravel-master in this example), or the result will be "404 not found".<br>
Furthermore, there is another way to navigate to the page :<br>
<pre>
  Route::get('users', 'UserController@getIndex');
</pre>
That means any request to <b>/users</b> will be navigated to the method <i>getIndex</i> within the <b>controller</b> <i>UserController</i>.<br>
For more details, check out <a href="#">controller</a> section.
