<h3>Create views</h3>
The next step is to create a <i>views</i> to present user data, the views file is located in <pre>app/views</pre>, including the html code.<br>
Now, we'll create two file: 
<pre>layout.blade.php</pre>
<code>
  <html>
	 <body>
		<h1>Larvel Quickstart</h1>
		
		@yield('content')
	 </body>
  </html> 
</code>
and <pre>users.blade.php</pre>.
<code>
  @extends('layout')
  
  @section('content')
	   Users!
  @stop
</code>
<i>"I am not familiar with the syntax in this moment, it's a little bit weird for me"</i><br>
Now, we have views, try to set up <pre>routes.php</pre> as following:
<code>
  Route::get('users', function()
  {
    return <b>View::make('users')</b>;
  });
</code>
