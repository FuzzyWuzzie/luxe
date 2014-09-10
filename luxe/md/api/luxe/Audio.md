
[![Logo](../../images/logo.png)](../../api/index.html)

---



<h1>Audio</h1>
<small>`luxe.Audio`</small>



---

`class`

---

&nbsp;
&nbsp;



<h3>Members</h3> <hr/>





<h3>Methods</h3> <hr/><span class="method apipage">
            <a name="create"><a class="lift" href="#create">create</a></a> <div class="clear"></div><code class="signature apipage">create(\_name:[String](#)<span></span>, \_file:[String](#)<span></span>, \_stream:[Bool](#)<span>=false</span>) : [snow.audio.Sound](#)</code><br/><span class="small_desc_flat">Create a named audio reference, with optional stream flag   
            **name** The name to assign this audio reference   
            **file** The asset file id from which the audio is loaded/streamed   
            **stream** Whether or not to stream the audio, default `false`   
            **returns** The `Sound` instance, but the audio API stores this, use the API to manipulate it by name.</span>
        </span>
    <span class="method apipage">
            <a name="uncreate"><a class="lift" href="#uncreate">uncreate</a></a> <div class="clear"></div><code class="signature apipage">uncreate(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Destroy a named audio reference.
            Use the reference directly with sound.destroy if you have an instance.</span>
        </span>
    <span class="method apipage">
            <a name="on"><a class="lift" href="#on">on</a></a> <div class="clear"></div><code class="signature apipage">on(\_name:[String](#)<span></span>, \_event:[String](#)<span></span>, \_handler:[snow.audio.Sound](#)&nbsp;-&gt; [Void](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Listen for an event on a named sound. `load` and `end` are valid</span>
        </span>
    <span class="method apipage">
            <a name="off"><a class="lift" href="#off">off</a></a> <div class="clear"></div><code class="signature apipage">off(\_name:[String](#)<span></span>, \_event:[String](#)<span></span>, \_handler:[snow.audio.Sound](#)&nbsp;-&gt; [Void](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Stop listening for an event on a named sound. See `on`</span>
        </span>
    <span class="method apipage">
            <a name="get"><a class="lift" href="#get">get</a></a> <div class="clear"></div><code class="signature apipage">get(\_name:[String](#)<span></span>) : [snow.audio.Sound](#)</code><br/><span class="small_desc_flat">Fetch a named audio reference   
            **name** The name to acquire audio reference   
            **returns** The `Sound` instance</span>
        </span>
    <span class="method apipage">
            <a name="exists"><a class="lift" href="#exists">exists</a></a> <div class="clear"></div><code class="signature apipage">exists(\_name:[String](#)<span></span>) : [Bool](#)</code><br/><span class="small_desc_flat">Determine whether a named audio reference exists   
            **name** The audio reference name to check   
            **returns** true/false</span>
        </span>
    <span class="method apipage">
            <a name="on_complete"><a class="lift" href="#on_complete">on\_complete</a></a> <div class="clear"></div><code class="signature apipage">on\_complete(\_name:[String](#)<span></span>, handler:[Dynamic](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Set the on complete handler for a named audio reference   
            **name** The audio reference name to assign to   
            **handler** The callback to call when playback is complete   
            **returns** nothing</span>
        </span>
    <span class="method apipage">
            <a name="loop"><a class="lift" href="#loop">loop</a></a> <div class="clear"></div><code class="signature apipage">loop(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Loop a named audio reference indefinitely. Use `stop` if needed.   
            **name** The audio reference name to loop   
            **returns** nothing</span>
        </span>
    <span class="method apipage">
            <a name="stop"><a class="lift" href="#stop">stop</a></a> <div class="clear"></div><code class="signature apipage">stop(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Stop a named audio reference from playing (or looping)   
            **name** The audio reference name to stop   
            **returns** nothing</span>
        </span>
    <span class="method apipage">
            <a name="play"><a class="lift" href="#play">play</a></a> <div class="clear"></div><code class="signature apipage">play(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Play a named audio reference   
            **name** The audio reference name to play   
            **returns** nothing</span>
        </span>
    <span class="method apipage">
            <a name="pause"><a class="lift" href="#pause">pause</a></a> <div class="clear"></div><code class="signature apipage">pause(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Pause a named audio reference   
            **name** The audio reference name to pause   
            **returns** nothing</span>
        </span>
    <span class="method apipage">
            <a name="toggle"><a class="lift" href="#toggle">toggle</a></a> <div class="clear"></div><code class="signature apipage">toggle(\_name:[String](#)<span></span>) : [Void](#)</code><br/><span class="small_desc_flat">Toggle a sound instance by name, pausing the sound or resuming it</span>
        </span>
    <span class="method apipage">
            <a name="volume"><a class="lift" href="#volume">volume</a></a> <div class="clear"></div><code class="signature apipage">volume(\_name:[String](#)<span></span>, \_volume:[Float](#)<span>=null</span>) : [Float](#)</code><br/><span class="small_desc_flat">get/set the volume of a named audio reference,   
            leave the second argument empty for get   
            **name** The audio reference name to adjust   
            **volume** A new volume value</span>
        </span>
    <span class="method apipage">
            <a name="pan"><a class="lift" href="#pan">pan</a></a> <div class="clear"></div><code class="signature apipage">pan(\_name:[String](#)<span></span>, \_pan:[Float](#)<span>=null</span>) : [Float](#)</code><br/><span class="small_desc_flat">get/set the pan of a named audio reference,   
            leave the second argument empty for get   
            **name** The audio reference name to adjust   
            **pan** A new pan value</span>
        </span>
    <span class="method apipage">
            <a name="pitch"><a class="lift" href="#pitch">pitch</a></a> <div class="clear"></div><code class="signature apipage">pitch(\_name:[String](#)<span></span>, \_pitch:[Float](#)<span>=null</span>) : [Float](#)</code><br/><span class="small_desc_flat">get/set the pitch of a named audio reference,   
            leave the second argument empty for get   
            **name** The audio reference name to adjust   
            **pitch** A new pitch value</span>
        </span>
    <span class="method apipage">
            <a name="position"><a class="lift" href="#position">position</a></a> <div class="clear"></div><code class="signature apipage">position(\_name:[String](#)<span></span>, \_position:[Float](#)<span>=null</span>) : [Float](#)</code><br/><span class="small_desc_flat">get/set the position in `seconds` of a named audio reference,   
            leave the second argument empty for get   
            **name** The audio reference name to adjust   
            **pan** A new pan value</span>
        </span>
    <span class="method apipage">
            <a name="duration"><a class="lift" href="#duration">duration</a></a> <div class="clear"></div><code class="signature apipage">duration(\_name:[String](#)<span></span>) : [Float](#)</code><br/><span class="small_desc_flat">get the position in seconds of a named audio reference   
            **name** The audio reference name to get</span>
        </span>
    





---

&nbsp;
&nbsp;
&nbsp;
&nbsp;