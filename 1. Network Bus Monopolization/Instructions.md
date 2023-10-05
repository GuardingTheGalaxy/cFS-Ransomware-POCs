
<h2>Attack vector 1</h2>
<p>This vector involves monopolizing the cFS internal network bus by overloading it with an infinite loop, called many times over by the main application. This exhausts resources, filling up the internal memory and preventing message delivery between processes, eventually shutting down the telemetry server.</p>

<p>To implement, please replace the native fm_app.c file in your local instance of cFS, located in:</p>
<code>/cfs/apps/fm/fsw/src/fm_app.c</code>
