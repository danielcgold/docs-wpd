---
title: API pages needing examples
todo_broken_links:
  note: 'During import MediaWiki could not find the following links, please fix and adjust this list.'
  links:
    - apis/file/MSStream
    - apis/webrtc/RTCPeerConnection/addstream
uri: 'WPD:Getting Started/examples/api'

---
Total: 428

<table>
<col width="33%" />
<col width="33%" />
<col width="33%" />
<thead>
<tr class="header">
<th align="left">Path</th>
<th align="left">Summary</th>
<th align="left">Modification date</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><a href="/apis/audio-video/video">apis/audio-video/video</a></td>
<td align="left">HTML Video element allows creator of a HTML document or view of a Web Application to embed a video for display when a user visits the view or opens HTML document in a web browser.</td>
<td align="left">27 April 2015 20:36:26</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/ScriptProcessorNode/onaudioprocess">apis/webaudio/ScriptProcessorNode/onaudioprocess</a></td>
<td align="left">An event listener which is called periodically for audio processing. An event of type <a href="/apis/webaudio/AudioProcessingEvent"><strong>AudioProcessingEvent</strong></a> will be passed to the event handler. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 19:49:55</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/ScriptProcessorNode/bufferSize">apis/webaudio/ScriptProcessorNode/bufferSize</a></td>
<td align="left">The size of the buffer (in sample-frames) which needs to be processed each time <a href="/apis/webaudio/ScriptProcessorNode/onaudioprocess"><strong>onaudioprocess</strong></a> is called. Legal values are 256, 512, 1024, 2048, 4096, 8192, and 16384. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 19:49:09</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/OscillatorNode/setWaveTable">apis/webaudio/OscillatorNode/setWaveTable</a></td>
<td align="left">Sets an arbitrary custom periodic waveform given a <a href="/apis/webaudio/WaveTable"><strong>WaveTable</strong></a>. <strong>Not in spec; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 19:17:53</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/OscillatorNode/playbackState">apis/webaudio/OscillatorNode/playbackState</a></td>
<td align="left">The playback state, initialized to UNSCHEDULED_STATE, progressing through SCHEDULED_STATE, PLAYING_STATE, and FINISHED_STATE. <strong>Not in spec; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 19:17:05</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/AudioProcessingEvent/playbackTime">apis/webaudio/AudioProcessingEvent/playbackTime</a></td>
<td align="left">The time when the audio will be played, in the same time coordinate system as <a href="/apis/webaudio/AudioContext/currentTime"><strong>AudioContext.currentTime</strong></a>. <a href="/apis/webaudio/AudioProcessingEvent/playbackTime"><strong>playbackTime</strong></a> allows for very tight synchronization between processing directly in JavaScript with the other events in the context's rendering graph. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:33:07</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/AudioProcessingEvent/outputBuffer">apis/webaudio/AudioProcessingEvent/outputBuffer</a></td>
<td align="left">An <a href="/apis/webaudio/AudioBuffer"><strong>AudioBuffer</strong></a> where the output audio data should be written. It will have a number of channels equal to the <strong>numberOfOutputChannels</strong> parameter of the <a href="/apis/webaudio/AudioContext/createScriptProcessor"><strong>createScriptProcessor()</strong></a> method. Script code within the scope of the <a href="/apis/webaudio/ScriptProcessorNode/onaudioprocess"><strong>onaudioprocess</strong></a> function is expected to modify the <strong>Float32Array</strong> arrays representing channel data in this <a href="/apis/webaudio/AudioBuffer"><strong>AudioBuffer</strong></a>. Any script modifications to this <a href="/apis/webaudio/AudioBuffer"><strong>AudioBuffer</strong></a> outside of this scope will not produce any audible effects. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:32:23</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/AudioProcessingEvent/node">apis/webaudio/AudioProcessingEvent/node</a></td>
<td align="left">The <a href="/apis/webaudio/ScriptProcessorNode"><strong>ScriptProcessorNode</strong></a> associated with this processing event. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:31:36</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/AudioProcessingEvent/inputBuffer">apis/webaudio/AudioProcessingEvent/inputBuffer</a></td>
<td align="left">An <a href="/apis/webaudio/AudioBuffer"><strong>AudioBuffer</strong></a> containing the input audio data. It will have a number of channels equal to the <strong>numberOfInputChannels</strong> parameter of the <a href="/apis/webaudio/AudioContext/createScriptProcessor"><strong>createScriptProcessor()</strong></a> method. This <a href="/apis/webaudio/AudioBuffer"><strong>AudioBuffer</strong></a> is only valid while in the scope of the <a href="/apis/webaudio/ScriptProcessorNode/onaudioprocess"><strong>onaudioprocess</strong></a> function. Its values will be meaningless outside of this scope. <strong>Deprecated; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:29:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/AudioParam/minValue">apis/webaudio/AudioParam/minValue</a></td>
<td align="left">Nominal minimum value. The value attribute may be set lower than this value. <strong>Not in spec; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:17:59</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/AudioParam/maxValue">apis/webaudio/AudioParam/maxValue</a></td>
<td align="left">Nominal maximum value. The value attribute may be set higher than this value. <strong>Not in spec; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:17:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/AudioParam/computedValue">apis/webaudio/AudioParam/computedValue</a></td>
<td align="left">The final value controlling the audio DSP, calculated at each time, which is either the value set directly to the value attribute or, if there are any scheduled parameter changes (automation events), the value as calculated from these events. <strong>Not in spec; deletion candidate. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">31 December 2014 18:06:57</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/AudioDestinationNode/numberOfChannels">apis/webaudio/AudioDestinationNode/numberOfChannels</a></td>
<td align="left">The number of channels of the destination's input. This value will default to 2, and may be set to any non-zero value less than or equal to <a href="/apis/webaudio/AudioDestinationNode/maxChannelCount"><strong>maxChannelCount</strong></a>. An exception will be thrown if this value is not within the valid range. <strong>Not in spec; deletion candidate. Possibly confused with AudioBuffer/numberOfChannels. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">29 December 2014 21:23:51</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webaudio/AudioContext/createWaveTable">apis/webaudio/AudioContext/createWaveTable</a></td>
<td align="left">Creates a <a href="/apis/webaudio/WaveTable"><strong>WaveTable</strong></a> representing a waveform containing arbitrary harmonic content. The real and imag parameters must be of type <strong>Float32Array</strong> of equal lengths greater than zero and less than or equal to 4096 or an exception will be thrown. These parameters specify the Fourier coefficients of a Fourier series representing the partials of a periodic waveform. The created <a href="/apis/webaudio/WaveTable"><strong>WaveTable</strong></a> will be used with an <a href="/apis/webaudio/OscillatorNode"><strong>OscillatorNode</strong></a> and will represent a normalized time-domain waveform having maximum absolute peak value of 1. Another way of saying this is that the generated waveform of an <a href="/apis/webaudio/OscillatorNode"><strong>OscillatorNode</strong></a> will have maximum peak value at 0dBFS. Conveniently, this corresponds to the full-range of the signal values used by the Web Audio API. Because the <a href="/apis/webaudio/WaveTable"><strong>WaveTable</strong></a> will be normalized on creation, the real and imag parameters represent relative values. <strong>Out of date; removed from spec. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">24 December 2014 18:56:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webaudio/AudioContext/activeSourceCount">apis/webaudio/AudioContext/activeSourceCount</a></td>
<td align="left">The number of <a href="/apis/webaudio/AudioBufferSourceNode"><strong>AudioBufferSourceNode</strong>s</a> that are currently playing. <strong>Out of date; removed from spec. See <a href="http://webaudio.github.io/web-audio-api/">http://webaudio.github.io/web-audio-api/</a>.</strong></td>
<td align="left">24 December 2014 18:03:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/VoidCallback/handleEvent">apis/filesystem/VoidCallback/handleEvent</a></td>
<td align="left">Indicates success of an asynchronous method. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:52:55</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/MetadataCallback/handleEvent">apis/filesystem/MetadataCallback/handleEvent</a></td>
<td align="left">Used to supply file or directory metadata as a response to a user query. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:51:53</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/LocalFileSystemSync/requestFileSystemSync">apis/filesystem/LocalFileSystemSync/requestFileSystemSync</a></td>
<td align="left">Requests a file system where data should be stored. You access a sandboxed file system by requesting a LocalFileSystemSync object from within a web worker using this global method, window.requestFileSystemSync(). <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:50:36</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/LocalFileSystemSync/resolveLocalFileSystemSyncURL">apis/filesystem/LocalFileSystemSync/resolveLocalFileSystemSyncURL</a></td>
<td align="left">Allows the user to look up the Entry for a file or directory referred to by a local URL. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:50:06</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/LocalFileSystem/requestFileSystem">apis/filesystem/LocalFileSystem/requestFileSystem</a></td>
<td align="left">Requests a file system where data should be stored. You access a sandboxed file system by requesting a LocalFileSystem object using this global method, window.requestFileSystem(). <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:49:04</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/LocalFileSystem/resolveLocalFileSystemURL">apis/filesystem/LocalFileSystem/resolveLocalFileSystemURL</a></td>
<td align="left">Allows the user to look up the Entry for a file or directory referred to by a local URL. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:48:26</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileWriterCallback/handleEvent">apis/filesystem/FileWriterCallback/handleEvent</a></td>
<td align="left">Used to supply a FileWriter as a response to a user query. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:47:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/FileSystemSync/name">apis/filesystem/FileSystemSync/name</a></td>
<td align="left">The name of the file system. The specifics of naming filesystems is unspecified, but a name must be unique across the list of exposed file systems. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:46:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileSystemSync/root">apis/filesystem/FileSystemSync/root</a></td>
<td align="left">The root directory of the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:45:21</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/FileSystemCallback/handleEvent">apis/filesystem/FileSystemCallback/handleEvent</a></td>
<td align="left">The file system was successfully obtained. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:43:24</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileSystem/name">apis/filesystem/FileSystem/name</a></td>
<td align="left">The name of the file system. The specifics of naming filesystems is unspecified, but a name must be unique across the list of exposed file systems. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:42:12</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/FileSystem/root">apis/filesystem/FileSystem/root</a></td>
<td align="left">The root directory of the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:41:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileEntrySync/createWriter">apis/filesystem/FileEntrySync/createWriter</a></td>
<td align="left">Creates a new FileWriterSync associated with the file that this FileEntrySync represents. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:40:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/FileEntrySync/file">apis/filesystem/FileEntrySync/file</a></td>
<td align="left">Returns a File that represents the current state of the file that this FileEntrySync represents. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:39:54</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileEntry/createWriter">apis/filesystem/FileEntry/createWriter</a></td>
<td align="left">Creates a new FileWriter associated with the file that this FileEntry represents. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:38:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/FileEntry/file">apis/filesystem/FileEntry/file</a></td>
<td align="left">Returns a File that represents the current state of the file that this FileEntry represents. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:38:13</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/FileCallback/handleEvent">apis/filesystem/FileCallback/handleEvent</a></td>
<td align="left">Used to supply a File as a response to a user query. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:36:32</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/ErrorCallback/handleEvent">apis/filesystem/ErrorCallback/handleEvent</a></td>
<td align="left">There was an error with the request. Details are provided by the err parameter. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">9 December 2014 17:35:06</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/onerror">apis/indexeddb/IDBTransaction/onerror</a></td>
<td align="left">The event handler for the error event.</td>
<td align="left">9 December 2014 01:04:18</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/error">apis/indexeddb/IDBTransaction/error</a></td>
<td align="left">Null if the transaction is not finished, is finished and successfully committed, or was aborted with the abort() function. Returns the same DOMError as the request object which caused the transaction to be aborted due to a failed request, or a DOMError for the transaction failure not due to a failed request (such as QuotaExceededError or UnknownError).</td>
<td align="left">9 December 2014 01:03:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBRequest/source">apis/indexeddb/IDBRequest/source</a></td>
<td align="left">The source of the request, such as an Index or a ObjectStore. If no source exists (such as when calling indexedDB.open()), it returns null.</td>
<td align="left">9 December 2014 01:03:11</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBRequest/transaction">apis/indexeddb/IDBRequest/transaction</a></td>
<td align="left">The transaction for the request. This property can be null for certain requests, such as for request returned from IDBFactory.open (You're just connecting to a database, so there is no transaction to return).</td>
<td align="left">9 December 2014 01:01:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/filesystem">apis/filesystem/EntrySync/filesystem</a></td>
<td align="left">The file system on which the EntrySync resides. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:08:32</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntrySync/fullPath">apis/filesystem/EntrySync/fullPath</a></td>
<td align="left">The full absolute path from the root to the EntrySync. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:08:11</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/isDirectory">apis/filesystem/EntrySync/isDirectory</a></td>
<td align="left">True if the EntrySync is a directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:07:49</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntrySync/isFile">apis/filesystem/EntrySync/isFile</a></td>
<td align="left">True if the EntrySync is a file. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:07:30</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/name">apis/filesystem/EntrySync/name</a></td>
<td align="left">The name of the EntrySync, excluding the path leading to it. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:07:08</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntrySync/copyTo">apis/filesystem/EntrySync/copyTo</a></td>
<td align="left">Copy an EntrySync to a different location on the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:06:45</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/getMetadata">apis/filesystem/EntrySync/getMetadata</a></td>
<td align="left">Look up metadata about this EntrySync. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:06:18</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntrySync/getParent">apis/filesystem/EntrySync/getParent</a></td>
<td align="left">Look up the parent DirectoryEntrySync containing this EntrySync. If this EntrySync is the root of its filesystem, its parent is itself. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:05:56</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/moveTo">apis/filesystem/EntrySync/moveTo</a></td>
<td align="left">Move an EntrySync to a different location on the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:05:29</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntrySync/remove">apis/filesystem/EntrySync/remove</a></td>
<td align="left">Deletes a file or directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:05:05</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/EntrySync/toURL">apis/filesystem/EntrySync/toURL</a></td>
<td align="left">Returns a URL that can be used to identify this EntrySync. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:04:43</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntryCallback/handleEvent">apis/filesystem/EntryCallback/handleEvent</a></td>
<td align="left">Used to supply an Entry as a response to a user query. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 18:01:03</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/filesystem">apis/filesystem/Entry/filesystem</a></td>
<td align="left">The file system on which the Entry resides. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:59:23</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/Entry/fullPath">apis/filesystem/Entry/fullPath</a></td>
<td align="left">The full absolute path from the root to the Entry. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:59:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/isDirectory">apis/filesystem/Entry/isDirectory</a></td>
<td align="left">True if the Entry is a directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:58:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/Entry/isFile">apis/filesystem/Entry/isFile</a></td>
<td align="left">True if the Entry is a file. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:57:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/name">apis/filesystem/Entry/name</a></td>
<td align="left">The name of the Entry, excluding the path leading to it. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:56:46</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/Entry/copyTo">apis/filesystem/Entry/copyTo</a></td>
<td align="left">Copy an Entry to a different location on the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:55:43</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/getMetadata">apis/filesystem/Entry/getMetadata</a></td>
<td align="left">Look up metadata about this Entry. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:55:17</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/Entry/getParent">apis/filesystem/Entry/getParent</a></td>
<td align="left">Look up the parent DirectoryEntry containing this Entry. If this Entry is the root of its filesystem, its parent is itself. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:54:50</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/moveTo">apis/filesystem/Entry/moveTo</a></td>
<td align="left">Move an Entry to a different location on the file system. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:54:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/Entry/remove">apis/filesystem/Entry/remove</a></td>
<td align="left">Deletes a file or directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:53:39</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/Entry/toURL">apis/filesystem/Entry/toURL</a></td>
<td align="left">Returns a URL that can be used to identify this Entry. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:53:03</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/DirectoryEntry/createReader">apis/filesystem/DirectoryEntry/createReader</a></td>
<td align="left">Creates a new DirectoryReader to read Entries from this Directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:19:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/DirectoryEntry/getDirectory">apis/filesystem/DirectoryEntry/getDirectory</a></td>
<td align="left">Creates or looks up a directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:19:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/DirectoryEntry/getFile">apis/filesystem/DirectoryEntry/getFile</a></td>
<td align="left">Creates or looks up a file. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:18:58</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/DirectoryEntry/removeRecursively">apis/filesystem/DirectoryEntry/removeRecursively</a></td>
<td align="left">Deletes a directory and all of its contents, if any. In the event of an error [e.g. trying to delete a directory that contains a file that cannot be removed], some of the contents of the directory may be deleted. It is an error to attempt to delete the root directory of a filesystem. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:18:29</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/DirectoryEntrySync/createReader">apis/filesystem/DirectoryEntrySync/createReader</a></td>
<td align="left">Creates a new DirectoryReaderSync to read EntrySyncs from this DirectorySync. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:17:08</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/DirectoryEntrySync/getDirectory">apis/filesystem/DirectoryEntrySync/getDirectory</a></td>
<td align="left">Creates or looks up a directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:16:45</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/DirectoryEntrySync/getFile">apis/filesystem/DirectoryEntrySync/getFile</a></td>
<td align="left">Creates or looks up a file. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:16:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/DirectoryEntrySync/removeRecursively">apis/filesystem/DirectoryEntrySync/removeRecursively</a></td>
<td align="left">Deletes a directory and all of its contents, if any. In the event of an error [e.g. trying to delete a directory that contains a file that cannot be removed], some of the contents of the directory may be deleted. It is an error to attempt to delete the root directory of a filesystem. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:15:40</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/DirectoryReader/readEntries">apis/filesystem/DirectoryReader/readEntries</a></td>
<td align="left">Read the next block of entries from this directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:14:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/filesystem/DirectoryReaderSync/readEntries">apis/filesystem/DirectoryReaderSync/readEntries</a></td>
<td align="left">Read the next block of entries from this directory. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:13:49</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/filesystem/EntriesCallback/handleEvent">apis/filesystem/EntriesCallback/handleEvent</a></td>
<td align="left">Used to supply an array of Entries as a response to a user query. <strong>Out of date; feature discontinued. See <a href="http://www.w3.org/TR/file-system-api/">http://www.w3.org/TR/file-system-api</a>.</strong></td>
<td align="left">5 December 2014 17:12:21</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/canvas/CanvasRenderingContext2D/ellipse">apis/canvas/CanvasRenderingContext2D/ellipse</a></td>
<td align="left">Draws the specified ellipse. If the object's path has any subpaths, this method adds a straight line from the last point in the subpath to the start point of the arc. Then, it adds the start and end points of the arc to the subpath, and connects them with an arc. <strong>Experimental, subject to change or removal; deletion candidate.</strong></td>
<td align="left">26 November 2014 20:38:58</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/canvas/CanvasRenderingContext2D/drawSystemFocusRing">apis/canvas/CanvasRenderingContext2D/drawSystemFocusRing</a></td>
<td align="left">Draws a focus ring of the appropriate style along the intended path, following platform conventions. <strong>Removed from spec; deletion candidate.</strong></td>
<td align="left">26 November 2014 20:34:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/canvas/CanvasRenderingContext2D/drawCustomFocusRing">apis/canvas/CanvasRenderingContext2D/drawCustomFocusRing</a></td>
<td align="left">Draw a focus ring of the appropriate style along the intended path, and sets result to <em>false</em>. <strong>Removed from spec; deletion candidate.</strong></td>
<td align="left">26 November 2014 20:11:30</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/KeyframeEffect/spacing">apis/web animations/KeyframeEffect/spacing</a></td>
<td align="left">The spacing mode to use for this animation effect.</td>
<td align="left">14 October 2014 14:08:49</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationEffect/composite">apis/web animations/AnimationEffect/composite</a></td>
<td align="left">The possible values of an animation effect's composition behavior are represented by the CompositeOperation enumeration.</td>
<td align="left">14 October 2014 14:04:27</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationEffect/iterationComposite">apis/web animations/AnimationEffect/iterationComposite</a></td>
<td align="left">The iteration composite operation property of this animation effect as specified by one of the IterationCompositeOperation enumeration values.</td>
<td align="left">14 October 2014 14:00:45</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/KeyframeEffect/getFrames">apis/web animations/KeyframeEffect/getFrames</a></td>
<td align="left">Returns the keyframes that make up this effect as a sequence of ComputedKeyframe objects.</td>
<td align="left">13 October 2014 23:50:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationEffect/name">apis/web animations/AnimationEffect/name</a></td>
<td align="left">A string used to identify the effect.</td>
<td align="left">13 October 2014 23:44:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/KeyframeEffect/setFrames">apis/web animations/KeyframeEffect/setFrames</a></td>
<td align="left">A Keyframe object or sequence of Keyframe objects used to replace the set of keyframes that make up this effect.</td>
<td align="left">13 October 2014 23:41:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/KeyframeEffect">apis/web animations/KeyframeEffect</a></td>
<td align="left">Keyframe animation effects are represented by the KeyframeEffect interface.</td>
<td align="left">13 October 2014 23:36:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/KeyframeEffect/constructor">apis/web animations/KeyframeEffect/constructor</a></td>
<td align="left">Creates a new KeyframeEffect object for the given set of keyframes.</td>
<td align="left">13 October 2014 23:35:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/easing">apis/web animations/AnimationTimingProperties/easing</a></td>
<td align="left">See the easing member of the AnimationTimingReadOnly interface. Unrecognized string values or values that correspond to a timing function that is not supported for the type of animation node to which this property is applied are treated as if the linear keyword was specified for the purpose of timing model calculations.</td>
<td align="left">13 October 2014 23:27:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/direction">apis/web animations/AnimationTimingProperties/direction</a></td>
<td align="left">See the direction member of the AnimationTimingReadOnly interface.</td>
<td align="left">13 October 2014 23:26:53</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/playbackRate">apis/web animations/AnimationTimingProperties/playbackRate</a></td>
<td align="left">See the playbackRate member of the AnimationTimingReadOnly interface.</td>
<td align="left">13 October 2014 23:26:15</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/duration">apis/web animations/AnimationTimingProperties/duration</a></td>
<td align="left">See the duration member of the AnimationTimingReadOnly interface. Real numbers less than zero, NaN values, and strings other than the lowercase value auto are treated the same as auto for the purpose of timing model calculations.</td>
<td align="left">13 October 2014 23:25:52</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/interations">apis/web animations/AnimationTimingProperties/interations</a></td>
<td align="left">See the iterations member of the AnimationTimingReadOnly interface. Values less than zero and NaN values are treated as the value 1.0 for the purpose of timing model calculations.</td>
<td align="left">13 October 2014 23:25:16</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/iterationStart">apis/web animations/AnimationTimingProperties/iterationStart</a></td>
<td align="left">See the iterationStart member of the AnimationTimingReadOnly interface.
<p>Values less than zero are clamped to zero for the purpose of timing model calculations.</p>
<p>Note that the value of iterations is effectively added to the iterationStart such that an animation node with an iterationStart of ‘0.5’ and iterations of ‘2’ would still repeat twice however it would begin and end half-way through the animation node’s iteration interval.</p>
Setting the iterationStart to a value greater than or equal to one is typically only useful in combination with an animation effect that has an iteration composite operation of ‘accumulate’.</td>
<td align="left">13 October 2014 23:24:35</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/fill">apis/web animations/AnimationTimingProperties/fill</a></td>
<td align="left">See the fill member of the AnimationTimingReadOnly interface.</td>
<td align="left">13 October 2014 23:24:05</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/endDelay">apis/web animations/AnimationTimingProperties/endDelay</a></td>
<td align="left">The specified end delay. See the description of the endDelay attribute on the AnimationTiming interface.</td>
<td align="left">13 October 2014 23:23:22</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties/delay">apis/web animations/AnimationTimingProperties/delay</a></td>
<td align="left">The specified start delay. See the description of the delay attribute on the AnimationTiming interface.</td>
<td align="left">13 October 2014 23:22:41</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingProperties">apis/web animations/AnimationTimingProperties</a></td>
<td align="left">The AnimationTimingProperties dictionary is encapsulates the timing properties of an AnimationNode so that they can be set in bulk (as in the constructor for Animation) or returned as a readonly snapshot (as in computedTiming).</td>
<td align="left">13 October 2014 23:14:45</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNode/previousSibling">apis/web animations/AnimationNode/previousSibling</a></td>
<td align="left">The previous sibling of this animation node.</td>
<td align="left">13 October 2014 23:12:15</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationNode/nextSibling">apis/web animations/AnimationNode/nextSibling</a></td>
<td align="left">The next sibling of this animation node.</td>
<td align="left">10 October 2014 03:22:15</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNode/replace">apis/web animations/AnimationNode/replace</a></td>
<td align="left">Replaces this AnimationNode with the passed in nodes.
<p>If there is no parent animation group, terminate these steps. If any of the animation nodes in nodes is an inclusive ancestor of the parent animation group throw a HierarchyRequestError exception and terminate these steps. Let reference child be the next sibling of this animation node not in nodes. Remove this animation node from its parent animation group.</p>
Insert nodes before reference child.</td>
<td align="left">10 October 2014 03:17:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationNode/after">apis/web animations/AnimationNode/after</a></td>
<td align="left">Inserts nodes after this animation node.
<p>If there is no parent animation group, terminate these steps. If any of the animation nodes in nodes is an inclusive ancestor of this animation node throw a HierarchyRequestError exception and terminate these steps. Let reference child be the next sibling of this animation node not in nodes.</p>
Insert nodes before reference child.</td>
<td align="left">10 October 2014 03:03:09</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNode/remove">apis/web animations/AnimationNode/remove</a></td>
<td align="left">Removes this animation node from its parent animation group or player.</td>
<td align="left">10 October 2014 03:01:23</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationNode/before">apis/web animations/AnimationNode/before</a></td>
<td align="left">Inserts nodes before this animation node.
<p>If there is no parent animation group, terminate these steps. If any of the animation nodes in nodes is an inclusive ancestor of this animation node throw a HierarchyRequestError exception and terminate these steps. Insert nodes before this animation node. Note that this definition precludes the following usage since node is an inclusive ancestor of itself:</p>
node.before(node); // throws HierarchyRequestError</td>
<td align="left">10 October 2014 02:58:43</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNode/computedTiming">apis/web animations/AnimationNode/computedTiming</a></td>
<td align="left">Returns the calculated timing properties for this animation node. This is comparable to the computed style of an Element, window.getComputedStyle(elem).
<p>Although several of the attributes of the this object are common to the AnimationTiming object returned by the timing attribute, they have the following differences:</p>
<p>duration – returns the calculated value of the iteration duration. If timing.duration is the string auto or any unsupported value, this attribute will return the current calculated value of the intrinsic iteration duration. fill – the auto value is replaced with the specific FillMode depending on the type of animation node (see §5.8.1 The FillMode enumeration).</p>
easing – unrecognised or unsupported values are replaced with the string linear.</td>
<td align="left">10 October 2014 02:48:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationGroup/clone">apis/web animations/AnimationGroup/clone</a></td>
<td align="left">Creates a deep copy of this AnimationGroup object using the following procedure.
<p>Let source be this AnimationGroup object, the object to be cloned. Let cloned timing be a new AnimationTimingProperties object whose members are assigned the value of the attribute with the same name on source.timing. Let cloned children be an empty sequence of AnimationNode objects. For each child in source.children, append the result of calling child.clone() to cloned children.</p>
Return a new AnimationGroup object created by calling the AnimationGroup constructor with parameters AnimationGroup(cloned children, cloned timing).</td>
<td align="left">10 October 2014 02:45:31</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationGroup/prepend">apis/web animations/AnimationGroup/prepend</a></td>
<td align="left">If any of the animation nodes in nodes is an inclusive ancestor of this animation node throw a HierarchyRequestError exception and terminate these steps. Insert nodes before the first child.</td>
<td align="left">10 October 2014 02:42:32</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationGroup/append">apis/web animations/AnimationGroup/append</a></td>
<td align="left">If any of the animation nodes in nodes is an inclusive ancestor of this animation node throw a HierarchyRequestError exception and terminate these steps. Insert nodes before null.</td>
<td align="left">10 October 2014 02:41:20</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationGroup/children">apis/web animations/AnimationGroup/children</a></td>
<td align="left">The list of child animation nodes in the group.</td>
<td align="left">10 October 2014 02:39:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationGroup/lastChild">apis/web animations/AnimationGroup/lastChild</a></td>
<td align="left">The last child of this animation group</td>
<td align="left">10 October 2014 02:38:32</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationGroup/firstChild">apis/web animations/AnimationGroup/firstChild</a></td>
<td align="left">The first child of this animation group.</td>
<td align="left">10 October 2014 02:38:08</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationGroup/constructor">apis/web animations/AnimationGroup/constructor</a></td>
<td align="left"></td>
<td align="left">10 October 2014 02:29:48</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/easing">apis/web animations/AnimationTimingReadOnly/easing</a></td>
<td align="left">The timing function used to scale the time to produce easing effects.</td>
<td align="left">9 October 2014 21:32:35</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/playbackRate">apis/web animations/AnimationTimingReadOnly/playbackRate</a></td>
<td align="left">The animation node’s playback rate property.</td>
<td align="left">9 October 2014 21:09:10</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/duration">apis/web animations/AnimationTimingReadOnly/duration</a></td>
<td align="left">The iteration duration which is a real number greater than or equal to zero (including positive infinity) representing the time taken to complete a single iteration of the animation node.</td>
<td align="left">9 October 2014 20:57:24</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/direction">apis/web animations/AnimationTimingReadOnly/direction</a></td>
<td align="left">The playback direction of the animation node as specified by one of the PlaybackDirection enumeration values.</td>
<td align="left">9 October 2014 20:56:07</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly">apis/web animations/AnimationTimingReadOnly</a></td>
<td align="left">Readonly class from which AnimationTiming classes are inherited.</td>
<td align="left">9 October 2014 20:55:33</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/endDelay">apis/web animations/AnimationTimingReadOnly/endDelay</a></td>
<td align="left">The end delay which represents the number of milliseconds from the end of an animation node’s active interval until the start time of any animation node that may follow, for example, in an animation sequence.</td>
<td align="left">9 October 2014 20:46:29</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/iterations">apis/web animations/AnimationTimingReadOnly/iterations</a></td>
<td align="left">The animation node’s iteration count property. A real number greater than or equal to zero (including positive infinity) representing the number of times to repeat the animation node.</td>
<td align="left">9 October 2014 20:45:31</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/iterationStart">apis/web animations/AnimationTimingReadOnly/iterationStart</a></td>
<td align="left">The animation node’s iteration start property. A finite real number greater than or equal to zero representing the number of iterations into the animation node at which to begin.</td>
<td align="left">9 October 2014 20:39:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/fill">apis/web animations/AnimationTimingReadOnly/fill</a></td>
<td align="left">The fill mode as specified by one of the FillMode enumeration values.
<p>When performing timing calculations the special value auto is expanded to one of the fill modes recognized by the timing model as follows,</p>
<p>If the animation node to which the fill mode is being is applied is an animation, Use none as the fill mode. Otherwise,</p>
Use both as the fill mode.</td>
<td align="left">9 October 2014 20:37:11</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimingReadOnly/delay">apis/web animations/AnimationTimingReadOnly/delay</a></td>
<td align="left">The start delay which represents the number of milliseconds from an animation node’s start time to the start of the active interval.</td>
<td align="left">9 October 2014 20:32:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/playState">apis/web animations/AnimationPlayer/playState</a></td>
<td align="left">The play state of this player.</td>
<td align="left">8 October 2014 22:58:20</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer">apis/web animations/AnimationPlayer</a></td>
<td align="left">Represents a single animation player. Players connect animation node, or source, to a timeline and provides playback controls.</td>
<td align="left">8 October 2014 22:53:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/AnimationPlayState">apis/web animations/AnimationPlayer/AnimationPlayState</a></td>
<td align="left">An enumeration of the various AnimationPlayer states.</td>
<td align="left">8 October 2014 22:50:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/reverse">apis/web animations/AnimationPlayer/reverse</a></td>
<td align="left">Inverts the playback rate of this player and seeks to the start of the source content if if has finished playing in the reversed direction using the reverse a player procedure for this object.</td>
<td align="left">8 October 2014 22:37:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/pause">apis/web animations/AnimationPlayer/pause</a></td>
<td align="left">Suspends the playback of this player by running the procedure to pause a player for this object.</td>
<td align="left">8 October 2014 22:36:17</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/play">apis/web animations/AnimationPlayer/play</a></td>
<td align="left">Unpauses the player and rewinds if it has finished playing using the procedure to play a player for this object.</td>
<td align="left">8 October 2014 22:35:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/finish">apis/web animations/AnimationPlayer/finish</a></td>
<td align="left">Seeks the player to the end of the source content in the current direction by running the finish a player procedure for this object.</td>
<td align="left">8 October 2014 22:34:24</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/cancel">apis/web animations/AnimationPlayer/cancel</a></td>
<td align="left">Clears all effects caused by this player and aborts its playback by running the cancel a player procedure for this object.</td>
<td align="left">8 October 2014 22:32:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/finished">apis/web animations/AnimationPlayer/finished</a></td>
<td align="left">Returns the current finished promise for this object.</td>
<td align="left">8 October 2014 22:30:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/ready">apis/web animations/AnimationPlayer/ready</a></td>
<td align="left">Returns the current ready promise for this object.</td>
<td align="left">8 October 2014 22:26:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/source">apis/web animations/AnimationPlayer/source</a></td>
<td align="left">The source content associated with this player. Setting this attribute updates the object’s source content using the procedure to set the source content of a player.</td>
<td align="left">8 October 2014 22:18:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/timeline">apis/web animations/AnimationPlayer/timeline</a></td>
<td align="left">The timeline associated with this player. Setting this attribute updates the object’s timeline using the procedure to set the timeline of a player.</td>
<td align="left">8 October 2014 22:09:11</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/playbackRate">apis/web animations/AnimationPlayer/playbackRate</a></td>
<td align="left">The playback rate of this player. Setting this attribute follows the procedure to update the player playback rate of this object to the new value.</td>
<td align="left">8 October 2014 22:05:00</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/currentTime">apis/web animations/AnimationPlayer/currentTime</a></td>
<td align="left">The current time of this player unless this player has a pending pause task, in which case this attribute returns null.</td>
<td align="left">8 October 2014 22:00:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/startTime">apis/web animations/AnimationPlayer/startTime</a></td>
<td align="left">Returns the start time of this player. Setting this attribute updates the player start time using the procedure to update the player start time of this object to the new value.</td>
<td align="left">8 October 2014 21:58:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationPlayer/constructor">apis/web animations/AnimationPlayer/constructor</a></td>
<td align="left">Constructs an new AnimationPlayer object.</td>
<td align="left">8 October 2014 21:54:05</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimeline/play">apis/web animations/AnimationTimeline/play</a></td>
<td align="left">Creates a new <a href="/apis/web_animations/AnimationPlayer"><strong>AnimationPlayer</strong></a> object associated with this timeline that begins playback as soon as it is ready.</td>
<td align="left">8 October 2014 21:48:09</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/Animation/constructor">apis/web animations/Animation/constructor</a></td>
<td align="left"></td>
<td align="left">8 October 2014 10:20:21</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimeline/getAnimationPlayers">apis/web animations/AnimationTimeline/getAnimationPlayers</a></td>
<td align="left">Returns the set of <a href="/apis/web_animations/AnimationPlayer"><strong>Animation Player</strong></a> objects associated with this timeline that have associated source content which is current or in effect.</td>
<td align="left">8 October 2014 09:37:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationTimeline/currentTime">apis/web animations/AnimationTimeline/currentTime</a></td>
<td align="left">Returns the time value for this timeline or null if this timeline is inactive.</td>
<td align="left">8 October 2014 09:32:27</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationEffect/clone">apis/web animations/AnimationEffect/clone</a></td>
<td align="left">Creates and returns a new object of the same type as this object's most-derived interface such that it will produce the same output as this object.</td>
<td align="left">8 October 2014 08:48:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/MotionPathEffect/MotionPathEffectOptions">apis/web animations/MotionPathEffect/MotionPathEffectOptions</a></td>
<td align="left"></td>
<td align="left">8 October 2014 08:38:56</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationPlayerEvent">apis/web animations/AnimationPlayerEvent</a></td>
<td align="left">Constructs a new AnimationPlayerEvent object as described in Constructing events in [DOM4]. <a href="http://www.w3.org/TR/dom/#constructing-events">http://www.w3.org/TR/dom/#constructing-events</a></td>
<td align="left">8 October 2014 08:13:52</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/MotionPathEffect">apis/web animations/MotionPathEffect</a></td>
<td align="left">Motion path animation effects are represented by the MotionPathEffect interface.</td>
<td align="left">8 October 2014 08:11:24</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationEffectapis/web_animations/AnimationEffect/CompositeOperation">apis/web animations/AnimationEffectapis/web animations/AnimationEffect/CompositeOperation</a></td>
<td align="left"></td>
<td align="left">8 October 2014 00:14:03</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationEffect/CompositeOperation">apis/web animations/AnimationEffect/CompositeOperation</a></td>
<td align="left">The possible values of an animation effect's composition behavior are represented by the CompositeOperation enumeration.</td>
<td align="left">8 October 2014 00:08:10</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTiming">apis/web animations/AnimationTiming</a></td>
<td align="left">Timing parameters for an AnimationNode are collected together under the AnimationTiming type.</td>
<td align="left">7 October 2014 23:48:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationNode/parent">apis/web animations/AnimationNode/parent</a></td>
<td align="left">The parent animation group of this animation node or null if this animation node does not have a parent animation group.</td>
<td align="left">7 October 2014 23:41:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNode/timing">apis/web animations/AnimationNode/timing</a></td>
<td align="left">Returns the input timing properties specified for this animation node. This is comparable to the specified style on an Element, elem.style.</td>
<td align="left">7 October 2014 23:37:35</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationGroup">apis/web animations/AnimationGroup</a></td>
<td align="left">Animation groups are represented by the AnimationGroup interface.</td>
<td align="left">7 October 2014 23:33:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationSequence">apis/web animations/AnimationSequence</a></td>
<td align="left">Animation sequences are represented by the AnimationSequence interface.</td>
<td align="left">7 October 2014 23:31:42</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/Animation/target">apis/web animations/Animation/target</a></td>
<td align="left"></td>
<td align="left">7 October 2014 22:59:20</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/Animation/effect">apis/web animations/Animation/effect</a></td>
<td align="left"></td>
<td align="left">7 October 2014 22:41:44</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/AnimationNode">apis/web animations/AnimationNode</a></td>
<td align="left">Animation nodes are represented in the Web Animations API by the AnimationNode interface.</td>
<td align="left">7 October 2014 21:35:43</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/CompositeOperation">apis/web animations/CompositeOperation</a></td>
<td align="left">The possible values of an animation effect’s composition behavior are represented by the CompositeOperation enumeration.</td>
<td align="left">7 October 2014 21:20:45</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/IterationCompositeOperation">apis/web animations/IterationCompositeOperation</a></td>
<td align="left">The possible values of an animation effect’s iteration composite operation are represented by the IterationCompositeOperation enumeration.</td>
<td align="left">7 October 2014 21:19:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationNodeList">apis/web animations/AnimationNodeList</a></td>
<td align="left">The sole reason this interface exists is to provide a familiar experience for authors familiar with DOM interfaces where child nodes are accessed via a children member.</td>
<td align="left">7 October 2014 21:12:56</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/web_animations/ComputedTimingProperties">apis/web animations/ComputedTimingProperties</a></td>
<td align="left"></td>
<td align="left">7 October 2014 21:07:51</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/web_animations/AnimationTimeline">apis/web animations/AnimationTimeline</a></td>
<td align="left">Representation of a timeline, including the document timeline.</td>
<td align="left">7 October 2014 13:38:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/audio-video/audio">apis/audio-video/audio</a></td>
<td align="left">The audio object is part of the HTML5 audio api. It extends the &lt;audio&gt; tag and allows users to access audio data. This enables the ability to manipulate or create new audio data.</td>
<td align="left">23 September 2014 16:55:18</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/audio-video/track">apis/audio-video/track</a></td>
<td align="left"></td>
<td align="left">23 September 2014 16:51:57</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/charging">apis/battery status/BatteryManager/charging</a></td>
<td align="left">Represents if the system's battery is charging.</td>
<td align="left">23 September 2014 16:42:38</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/chargingTime">apis/battery status/BatteryManager/chargingTime</a></td>
<td align="left">Represents the time remaining in seconds until the system's battery is fully charged.</td>
<td align="left">23 September 2014 16:42:08</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/chargingchange">apis/battery status/BatteryManager/chargingchange</a></td>
<td align="left">Fired when the battery charging state is updated.</td>
<td align="left">23 September 2014 16:41:27</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/chargingtimechange">apis/battery status/BatteryManager/chargingtimechange</a></td>
<td align="left">Fired when the battery charging time is updated.</td>
<td align="left">23 September 2014 16:40:54</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/dischargingTime">apis/battery status/BatteryManager/dischargingTime</a></td>
<td align="left">Represents the time remaining in seconds until the system's battery is completely discharged and the system is about to be suspended.</td>
<td align="left">23 September 2014 16:40:10</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/dischargingtimechange">apis/battery status/BatteryManager/dischargingtimechange</a></td>
<td align="left">Fired when the battery discharging time is updated.</td>
<td align="left">23 September 2014 16:39:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/NavigatorBattery/battery">apis/battery status/NavigatorBattery/battery</a></td>
<td align="left">The object that exposes the battery status information.</td>
<td align="left">23 September 2014 16:37:29</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/level">apis/battery status/BatteryManager/level</a></td>
<td align="left">Represents the current battery level scaled from 0 to 1.0.</td>
<td align="left">23 September 2014 16:37:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/levelchange">apis/battery status/BatteryManager/levelchange</a></td>
<td align="left">Fired when the battery level is updated.</td>
<td align="left">23 September 2014 16:36:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/onchargingchange">apis/battery status/BatteryManager/onchargingchange</a></td>
<td align="left">Handles the chargingchange event.</td>
<td align="left">23 September 2014 16:34:29</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/onchargingtimechange">apis/battery status/BatteryManager/onchargingtimechange</a></td>
<td align="left">Handles the chargingtimechange event.</td>
<td align="left">23 September 2014 16:34:01</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/battery_status/BatteryManager/ondischargingtimechange">apis/battery status/BatteryManager/ondischargingtimechange</a></td>
<td align="left">Handles the dischargingtimechange event.</td>
<td align="left">23 September 2014 16:33:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/battery_status/BatteryManager/onlevelchange">apis/battery status/BatteryManager/onlevelchange</a></td>
<td align="left">Handles the levelchange event.</td>
<td align="left">23 September 2014 16:32:47</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/file/FileError">apis/file/FileError</a></td>
<td align="left">Represents an error that occurs while using the FileReader interface. Obsolete per latest specification. Use <a href="/dom/DOMError">DOMError</a> instead.</td>
<td align="left">22 September 2014 18:16:20</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/file/MSStreamError">apis/file/MSStreamError</a></td>
<td align="left">The MSStreamError object reports file-related errors asynchronously. Obsolete per latest specification. Use <a href="/dom/DOMError">DOMError</a> instead.</td>
<td align="left">22 September 2014 18:07:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/file/MSStreamReader">apis/file/MSStreamReader</a></td>
<td align="left">Creates random access data (Blob) from an MSStream object.</td>
<td align="left">22 September 2014 18:06:58</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/file/MSStreamReader/onabort">apis/file/MSStreamReader/onabort</a></td>
<td align="left">Indicates that the read has been aborted (for example, by calling <strong>abort()</strong>).</td>
<td align="left">22 September 2014 18:06:31</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/file/MSStreamReader/readAsBlob">apis/file/MSStreamReader/readAsBlob</a></td>
<td align="left">Performs an asynchronous read of an <a href="/w/index.php?title=apis/file/MSStream&amp;action=edit&amp;redlink=1">MSStream</a> object in order to create a <a href="/apis/file/Blob">Blob</a> object.</td>
<td align="left">22 September 2014 18:05:15</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/file/MSStreamReader/readAsText">apis/file/MSStreamReader/readAsText</a></td>
<td align="left">Returns partial Blob data representing the number of bytes currently loaded (as a fraction of the total), decoded into memory according to the encoding determination.</td>
<td align="left">22 September 2014 18:04:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/file/URL/revokeObjectURL">apis/file/URL/revokeObjectURL</a></td>
<td align="left">Revokes a URL from a document and frees the object associated with that URL.</td>
<td align="left">22 September 2014 18:00:10</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/ImageCapture/getFrame">apis/image capture/ImageCapture/getFrame</a></td>
<td align="left">Gathers data from the VideoStreamTrack into a ImageData object.</td>
<td align="left">18 September 2014 18:11:59</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/ImageCapture/onerror">apis/image capture/ImageCapture/onerror</a></td>
<td align="left">Register/unregister for Image Capture error events of type ImageCaptureErrorEvent.</td>
<td align="left">18 September 2014 18:11:33</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/ImageCapture/onframegrab">apis/image capture/ImageCapture/onframegrab</a></td>
<td align="left">Register/unregister for frame capture events of type FrameGrabEvent.</td>
<td align="left">18 September 2014 18:11:08</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/ImageCapture/onphoto">apis/image capture/ImageCapture/onphoto</a></td>
<td align="left">Register/unregister for photo events of type BlobEvent.</td>
<td align="left">18 September 2014 18:10:41</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/ImageCapture/onphotosettingschange">apis/image capture/ImageCapture/onphotosettingschange</a></td>
<td align="left">Register/unregister for photo settings change events of type SettingsChangeEvent.</td>
<td align="left">18 September 2014 18:10:13</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettingsOptions">apis/image capture/PhotoSettingsOptions</a></td>
<td align="left">Provides the photo-specific settings options and current settings values.</td>
<td align="left">18 September 2014 18:09:29</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/ImageCapture/photoSettingsOptions">apis/image capture/ImageCapture/photoSettingsOptions</a></td>
<td align="left">Describes current photo settings.</td>
<td align="left">18 September 2014 18:07:41</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/ImageCapture/setOptions">apis/image capture/ImageCapture/setOptions</a></td>
<td align="left">Applies the settings specified by the PhotoSettings object passed by parameter.</td>
<td align="left">18 September 2014 18:07:08</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/ImageCapture/takePhoto">apis/image capture/ImageCapture/takePhoto</a></td>
<td align="left">Gathers data from the VideoStreamTrack into a Blob containing a single still image.</td>
<td align="left">18 September 2014 18:06:24</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/ImageCapture/videoStreamTrack">apis/image capture/ImageCapture/videoStreamTrack</a></td>
<td align="left">The MediaStream passed into the constructor.</td>
<td align="left">18 September 2014 18:05:46</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/autoExposureMode">apis/image capture/PhotoSettings/autoExposureMode</a></td>
<td align="left">This reflects the desired auto exposure mode setting.</td>
<td align="left">18 September 2014 18:04:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/autoWhiteBalanceMode">apis/image capture/PhotoSettings/autoWhiteBalanceMode</a></td>
<td align="left">This reflects whether automatic White Balance Mode selection is desired.</td>
<td align="left">18 September 2014 18:02:53</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/brightness">apis/image capture/PhotoSettings/brightness</a></td>
<td align="left">This reflects the desired brightness setting of the camera.</td>
<td align="left">18 September 2014 18:02:24</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/contrast">apis/image capture/PhotoSettings/contrast</a></td>
<td align="left">This reflects the desired contrast setting of the camera.</td>
<td align="left">18 September 2014 18:01:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/exposureCompensation">apis/image capture/PhotoSettings/exposureCompensation</a></td>
<td align="left">This reflects the desired exposure compensation setting.</td>
<td align="left">18 September 2014 18:01:31</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/imageHeight">apis/image capture/PhotoSettings/imageHeight</a></td>
<td align="left">This reflects the desired image height.</td>
<td align="left">18 September 2014 18:01:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/imageWidth">apis/image capture/PhotoSettings/imageWidth</a></td>
<td align="left">This reflects the desired image width.</td>
<td align="left">18 September 2014 18:00:35</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/iso">apis/image capture/PhotoSettings/iso</a></td>
<td align="left">This reflects the desired camera ISO setting.</td>
<td align="left">18 September 2014 17:59:46</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/redEyeReduction">apis/image capture/PhotoSettings/redEyeReduction</a></td>
<td align="left">This reflects whether camera red eye reduction is desired.</td>
<td align="left">18 September 2014 17:59:17</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/saturation">apis/image capture/PhotoSettings/saturation</a></td>
<td align="left">This reflects the desired saturation setting of the camera.</td>
<td align="left">18 September 2014 17:58:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/image_capture/PhotoSettings/whiteBalanceMode">apis/image capture/PhotoSettings/whiteBalanceMode</a></td>
<td align="left">This reflects the desired white balance mode setting.</td>
<td align="left">18 September 2014 17:58:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/image_capture/PhotoSettings/sharpness">apis/image capture/PhotoSettings/sharpness</a></td>
<td align="left">This reflects the desired sharpness setting of the camera.</td>
<td align="left">18 September 2014 17:57:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBCursor/delete">apis/indexeddb/IDBCursor/delete</a></td>
<td align="left">Returns an IDBRequest object and, in a separate thread, deletes the record at the cursor's position, without changing the cursor's position. Once the record is deleted, the cursor's value is set to null.</td>
<td align="left">17 September 2014 21:33:55</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBCursor/direction">apis/indexeddb/IDBCursor/direction</a></td>
<td align="left">Indicates the direction of travel within a cursor.</td>
<td align="left">17 September 2014 21:33:20</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBCursor/key">apis/indexeddb/IDBCursor/key</a></td>
<td align="left">The key value for the record currently displayed by the cursor.</td>
<td align="left">17 September 2014 21:32:03</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBCursor/primaryKey">apis/indexeddb/IDBCursor/primaryKey</a></td>
<td align="left">Returns the cursor's current effective key.</td>
<td align="left">17 September 2014 21:30:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBCursor/source">apis/indexeddb/IDBCursor/source</a></td>
<td align="left">On getting, returns the IDBObjectStore or IDBIndex that the cursor is iterating. This function never returns null or throws an exception, even if the cursor is currently being iterated, has iterated past its end, or its transaction is not active.</td>
<td align="left">17 September 2014 21:30:23</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBCursor/update">apis/indexeddb/IDBCursor/update</a></td>
<td align="left">Creates a structured clone of the value parameter.</td>
<td align="left">17 September 2014 21:29:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBCursorWithValue/value">apis/indexeddb/IDBCursorWithValue/value</a></td>
<td align="left"></td>
<td align="left">17 September 2014 21:24:45</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/deleteObjectStore">apis/indexeddb/IDBDatabase/deleteObjectStore</a></td>
<td align="left">Destroys an object store with the given name as well as all indexes that are referencing that object store.</td>
<td align="left">17 September 2014 21:19:33</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/name">apis/indexeddb/IDBDatabase/name</a></td>
<td align="left">Name of the connected database.</td>
<td align="left">17 September 2014 21:12:53</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/objectStoreNames">apis/indexeddb/IDBDatabase/objectStoreNames</a></td>
<td align="left">Returns a list of names of the object stores currently in the connected database.</td>
<td align="left">17 September 2014 21:12:21</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBDatabaseException">apis/indexeddb/IDBDatabaseException</a></td>
<td align="left">Not supported.</td>
<td align="left">17 September 2014 21:11:34</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBDatabaseException/code">apis/indexeddb/IDBDatabaseException/code</a></td>
<td align="left">Not supported.</td>
<td align="left">17 September 2014 21:11:17</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBDatabaseException/message">apis/indexeddb/IDBDatabaseException/message</a></td>
<td align="left">Not supported.</td>
<td align="left">17 September 2014 21:10:58</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/setVersion">apis/indexeddb/IDBDatabase/setVersion</a></td>
<td align="left">Deletion candidate. Not in spec: <a href="http://www.w3.org/TR/IndexedDB/">http://www.w3.org/TR/IndexedDB/</a></td>
<td align="left">17 September 2014 21:10:10</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/transaction">apis/indexeddb/IDBDatabase/transaction</a></td>
<td align="left">Execute the steps for creating a transaction in a sychronous fashion.</td>
<td align="left">17 September 2014 21:09:00</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBDatabase/version">apis/indexeddb/IDBDatabase/version</a></td>
<td align="left">Returns the version of the database when this IDBDatabaseSync instance was created.</td>
<td align="left">17 September 2014 21:06:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBIndex/count">apis/indexeddb/IDBIndex/count</a></td>
<td align="left">Runs the steps for asynchronously executing a request and returns the IDBRequest created by these steps.</td>
<td align="left">17 September 2014 20:53:59</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBIndex/get">apis/indexeddb/IDBIndex/get</a></td>
<td align="left">Runs the steps for asynchronously executing a request and returns the IDBRequest created by these steps.</td>
<td align="left">17 September 2014 20:52:56</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBIndex/keyPath">apis/indexeddb/IDBIndex/keyPath</a></td>
<td align="left">The key path of this index. If null, this index is not auto-populated.</td>
<td align="left">17 September 2014 20:52:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBIndex/multiEntry">apis/indexeddb/IDBIndex/multiEntry</a></td>
<td align="left">Affects how the index behaves when the result of evaluating the index's key path yields an array. If true, there is one record in the index for each item in an array of keys. If false, then there is one record for each key that is an array.</td>
<td align="left">17 September 2014 20:51:51</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBIndex/name">apis/indexeddb/IDBIndex/name</a></td>
<td align="left">The name of this index.</td>
<td align="left">17 September 2014 20:51:24</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBIndex/objectStore">apis/indexeddb/IDBIndex/objectStore</a></td>
<td align="left">Returns a reference to the IDBObjectStore instance for the referenced object store in this IDBIndex's transaction.</td>
<td align="left">17 September 2014 18:20:55</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBIndex/openCursor">apis/indexeddb/IDBIndex/openCursor</a></td>
<td align="left">Creates a cursor.</td>
<td align="left">17 September 2014 18:20:13</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBIndex/openKeyCursor">apis/indexeddb/IDBIndex/openKeyCursor</a></td>
<td align="left">Creates a cursor.</td>
<td align="left">17 September 2014 18:19:27</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBIndex/unique">apis/indexeddb/IDBIndex/unique</a></td>
<td align="left">Provides the unique flag of this index.</td>
<td align="left">17 September 2014 18:17:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/lower">apis/indexeddb/IDBKeyRange/lower</a></td>
<td align="left">This value is the lower-bound of the key range.</td>
<td align="left">17 September 2014 18:13:43</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/lowerBound">apis/indexeddb/IDBKeyRange/lowerBound</a></td>
<td align="left">Creates and returns a new key range with lower set to lower, lowerOpen set to open, upper set to undefined and and upperOpen set to true.</td>
<td align="left">17 September 2014 18:12:24</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/lowerOpen">apis/indexeddb/IDBKeyRange/lowerOpen</a></td>
<td align="left">Returns false if the lower-bound value is included in the key range. Returns true if the lower-bound value is excluded from the key range.</td>
<td align="left">17 September 2014 18:11:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/only">apis/indexeddb/IDBKeyRange/only</a></td>
<td align="left">Creates and returns a new key range with both lower and upper set to value and both lowerOpen and upperOpen set to false.</td>
<td align="left">17 September 2014 18:10:58</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/upperBound">apis/indexeddb/IDBKeyRange/upperBound</a></td>
<td align="left">Creates and returns a new key range with lower set to undefined, lowerOpen set to true, upper set to upper and and upperOpen set to open.</td>
<td align="left">17 September 2014 18:10:10</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBKeyRange/upperOpen">apis/indexeddb/IDBKeyRange/upperOpen</a></td>
<td align="left">Returns false if the upper-bound value is included in the key range. Returns true if the upper-bound value is excluded from the key range.</td>
<td align="left">17 September 2014 18:09:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/autoIncrement">apis/indexeddb/IDBObjectStore/autoIncrement</a></td>
<td align="left">Provides the auto increment flag for this object store.</td>
<td align="left">17 September 2014 18:05:35</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/count">apis/indexeddb/IDBObjectStore/count</a></td>
<td align="left">The count method returns the number of records in an object store.</td>
<td align="left">17 September 2014 18:03:58</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/openCursor">apis/indexeddb/IDBObjectStore/openCursor</a></td>
<td align="left">Creates a cursor.</td>
<td align="left">17 September 2014 17:57:23</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/get">apis/indexeddb/IDBObjectStore/get</a></td>
<td align="left">Runs the steps for asynchronously executing a request and returns the IDBRequest created by these steps.</td>
<td align="left">17 September 2014 17:49:59</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/index">apis/indexeddb/IDBObjectStore/index</a></td>
<td align="left">Returns an IDBIndex representing an index that is part of the object store.</td>
<td align="left">17 September 2014 17:47:26</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/indexNames">apis/indexeddb/IDBObjectStore/indexNames</a></td>
<td align="left">Provides a list of the names of indexes on objects in this object store.</td>
<td align="left">17 September 2014 17:45:30</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/keyPath">apis/indexeddb/IDBObjectStore/keyPath</a></td>
<td align="left">Provides the key path of this object store.</td>
<td align="left">17 September 2014 17:44:49</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/name">apis/indexeddb/IDBObjectStore/name</a></td>
<td align="left">Provides the name of this object store.</td>
<td align="left">17 September 2014 17:44:09</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/put">apis/indexeddb/IDBObjectStore/put</a></td>
<td align="left">Creates a structured clone of the value parameter.</td>
<td align="left">17 September 2014 17:40:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBObjectStore/transaction">apis/indexeddb/IDBObjectStore/transaction</a></td>
<td align="left">Returns the transaction this object store belongs to.</td>
<td align="left">17 September 2014 17:33:08</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBOpenDBRequest/onUpgradeNeeded">apis/indexeddb/IDBOpenDBRequest/onUpgradeNeeded</a></td>
<td align="left">The event handler for the upgrade needed event.</td>
<td align="left">17 September 2014 17:28:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBOpenDBRequest/onblocked">apis/indexeddb/IDBOpenDBRequest/onblocked</a></td>
<td align="left">The event handler for the blocked event. This event is triggered when the upgradeneeded should be triggered because of a version change but the database is still in use (ie not closed) somewhere, even after the versionchange event was sent.</td>
<td align="left">17 September 2014 17:28:20</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBRequest/error">apis/indexeddb/IDBRequest/error</a></td>
<td align="left">The error codes returned under certain conditions.</td>
<td align="left">17 September 2014 17:25:23</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBRequest/onerror">apis/indexeddb/IDBRequest/onerror</a></td>
<td align="left">The event handler for the error event.</td>
<td align="left">17 September 2014 17:23:51</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBRequest/onsuccess">apis/indexeddb/IDBRequest/onsuccess</a></td>
<td align="left">The event handler for the success event.</td>
<td align="left">17 September 2014 17:23:26</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBRequest/readyState">apis/indexeddb/IDBRequest/readyState</a></td>
<td align="left">The state of the request. Every request starts in the pending state. The state changes to done when the request completes successfully or when an error occurs.</td>
<td align="left">17 September 2014 17:23:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBRequest/result">apis/indexeddb/IDBRequest/result</a></td>
<td align="left">Returns the result of the request. If the the request failed and the result is not available, the DOMException InvalidStateError exception is thrown.</td>
<td align="left">17 September 2014 17:22:19</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/mode">apis/indexeddb/IDBTransaction/mode</a></td>
<td align="left">The mode for isolating access to data in the object stores that are in the scope of the transaction. For possible values, see Return Value, below. The default value is readonly.</td>
<td align="left">17 September 2014 17:16:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/db">apis/indexeddb/IDBTransaction/db</a></td>
<td align="left">The database connection of which this transaction is a part.</td>
<td align="left">17 September 2014 17:16:01</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/objectStore">apis/indexeddb/IDBTransaction/objectStore</a></td>
<td align="left">Returns an object store that has already been added to the scope of this transaction.</td>
<td align="left">17 September 2014 17:12:19</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/onabort">apis/indexeddb/IDBTransaction/onabort</a></td>
<td align="left">The event handler for the onabort event.</td>
<td align="left">17 September 2014 17:11:46</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBTransaction/oncomplete">apis/indexeddb/IDBTransaction/oncomplete</a></td>
<td align="left">The event handler for the oncomplete event.</td>
<td align="left">17 September 2014 17:11:22</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBVersionChangeEvent/newVersion">apis/indexeddb/IDBVersionChangeEvent/newVersion</a></td>
<td align="left">Returns the new version of the database, which is the version specified by the open request.</td>
<td align="left">17 September 2014 17:05:32</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/IDBVersionChangeEvent/oldVersion">apis/indexeddb/IDBVersionChangeEvent/oldVersion</a></td>
<td align="left">Returns the old version of the database.</td>
<td align="left">17 September 2014 17:05:07</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/indexeddb/IDBVersionChangeRequest/onblocked">apis/indexeddb/IDBVersionChangeRequest/onblocked</a></td>
<td align="left">The event handler for the blocked event.</td>
<td align="left">17 September 2014 17:01:43</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/indexeddb/indexedDB/open">apis/indexeddb/indexedDB/open</a></td>
<td align="left">Opens a database. See <a href="/apis/indexeddb/IDBFactory/open">apis/indexeddb/IDBFactory/open</a></td>
<td align="left">17 September 2014 16:59:46</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/internationalization/Intl/Collator">apis/internationalization/Intl/Collator</a></td>
<td align="left"></td>
<td align="left">16 September 2014 17:51:06</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/internationalization/Intl/DateTimeFormat">apis/internationalization/Intl/DateTimeFormat</a></td>
<td align="left"></td>
<td align="left">16 September 2014 17:50:32</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/internationalization/Intl/NumberFormat">apis/internationalization/Intl/NumberFormat</a></td>
<td align="left"></td>
<td align="left">16 September 2014 17:49:50</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/addtrack">apis/media capture and streams/MediaStream/addtrack</a></td>
<td align="left">This event is fired when a track is added to the MediaStream.</td>
<td align="left">16 September 2014 17:25:54</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/ended">apis/media capture and streams/MediaStream/ended</a></td>
<td align="left">Is true if the MediaStream has finished, false otherwise.</td>
<td align="left">16 September 2014 17:25:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/id">apis/media capture and streams/MediaStream/id</a></td>
<td align="left">A globally unique identifier string, initialized when the MediaStream object is created.</td>
<td align="left">16 September 2014 17:24:42</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/onaddtrack">apis/media capture and streams/MediaStream/onaddtrack</a></td>
<td align="left">Handles the addtrack event when fired on the MediaStream object.</td>
<td align="left">16 September 2014 17:24:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/onended">apis/media capture and streams/MediaStream/onended</a></td>
<td align="left">Handles the ended event when fired on the MediaStream object.</td>
<td align="left">16 September 2014 17:23:36</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/onremovetrack">apis/media capture and streams/MediaStream/onremovetrack</a></td>
<td align="left">Handles the removetrack event when fired on the MediaStream object.</td>
<td align="left">16 September 2014 17:22:40</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStream/removetrack">apis/media capture and streams/MediaStream/removetrack</a></td>
<td align="left">This event is fired when a track is removed from the MediaStream.</td>
<td align="left">16 September 2014 17:21:55</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/applyConstraints">apis/media capture and streams/MediaStreamTrack/applyConstraints</a></td>
<td align="left">Replaces all existing constraints with the provided constraints, if existing constraints exist. Otherwise, it applies the newly provided constraints to the track.</td>
<td align="left">16 September 2014 17:20:19</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/capabilities">apis/media capture and streams/MediaStreamTrack/capabilities</a></td>
<td align="left">Returns a dictionary with all of the capabilities for the track type.</td>
<td align="left">16 September 2014 17:19:48</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/clone">apis/media capture and streams/MediaStreamTrack/clone</a></td>
<td align="left">Clones the given MediaStreamTrack.</td>
<td align="left">16 September 2014 17:19:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/constraints">apis/media capture and streams/MediaStreamTrack/constraints</a></td>
<td align="left">Returns the complete constraints object associated with the track. If no mandatory constraints have been defined, the mandatory field will not be present (it will be undefined). If no optional constraints have been defined, the optional field will not be present (it will be undefined). If neither optional, nor mandatory constraints have been created, the value null is returned.</td>
<td align="left">16 September 2014 17:18:42</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/enabled">apis/media capture and streams/MediaStreamTrack/enabled</a></td>
<td align="left">Enables the track if the new value is true, and disable it otherwise.</td>
<td align="left">16 September 2014 17:17:58</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/id">apis/media capture and streams/MediaStreamTrack/id</a></td>
<td align="left">A globally unique identifier string, initialized when the MediaStreamTrack object is created.</td>
<td align="left">16 September 2014 17:17:32</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/kind">apis/media capture and streams/MediaStreamTrack/kind</a></td>
<td align="left">Returns the string &quot;audio&quot; if the object represents an audio track or &quot;video&quot; if object represents a video track.</td>
<td align="left">16 September 2014 17:16:51</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/onmute">apis/media capture and streams/MediaStreamTrack/onmute</a></td>
<td align="left">Handles the mute event when fired on the MediaStreamTrack object.</td>
<td align="left">16 September 2014 16:54:30</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/onoverconstrained">apis/media capture and streams/MediaStreamTrack/onoverconstrained</a></td>
<td align="left">Handles the overcontrained event when fired on the MediaStreamTrack object.</td>
<td align="left">16 September 2014 16:53:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/onstarted">apis/media capture and streams/MediaStreamTrack/onstarted</a></td>
<td align="left">Handles the started event when fired on the MediaStreamTrack object.</td>
<td align="left">16 September 2014 16:52:50</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/label">apis/media capture and streams/MediaStreamTrack/label</a></td>
<td align="left">Returns the label of the object’s corresponding track, if any. If the corresponding track has or had no label, it returns the empty string.</td>
<td align="left">16 September 2014 16:51:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/mute">apis/media capture and streams/MediaStreamTrack/mute</a></td>
<td align="left">This event fires when the MediaStreamTrack object's source is temporarily unable to provide data.</td>
<td align="left">16 September 2014 16:51:08</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/muted">apis/media capture and streams/MediaStreamTrack/muted</a></td>
<td align="left">Returns true if the track is muted, and false otherwise.</td>
<td align="left">16 September 2014 16:50:32</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/onended">apis/media capture and streams/MediaStreamTrack/onended</a></td>
<td align="left">Handles the ended event when fired on the MediaStreamTrack object.</td>
<td align="left">16 September 2014 16:49:49</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/onunmute">apis/media capture and streams/MediaStreamTrack/onunmute</a></td>
<td align="left">Handles the unmute event when fired on the MediaStreamTrack object.</td>
<td align="left">16 September 2014 16:49:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/overconstrained">apis/media capture and streams/MediaStreamTrack/overconstrained</a></td>
<td align="left">This event fires asynchronously for each affected track (when multiple tracks share the same source) after the user agent has evaluated the current constraints against a given sourceId and is not able to configure the source within the limitations established by the union of imposed constraints.</td>
<td align="left">16 September 2014 16:48:42</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/readonly">apis/media capture and streams/MediaStreamTrack/readonly</a></td>
<td align="left">Returns true If the track (audio or video) is backed by a read-only source such as a file, or the track source is a local microphone or camera, but is shared so that this track cannot modify any of the source's settings. Returns false otherwise.</td>
<td align="left">16 September 2014 16:48:13</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/readyState">apis/media capture and streams/MediaStreamTrack/readyState</a></td>
<td align="left">Returns the state of the track.</td>
<td align="left">16 September 2014 16:47:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/remote">apis/media capture and streams/MediaStreamTrack/remote</a></td>
<td align="left">Returns true if the track is sourced by an RTCPeerConnection. Returns false otherwise.</td>
<td align="left">16 September 2014 16:46:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/started">apis/media capture and streams/MediaStreamTrack/started</a></td>
<td align="left">This event fires when the MediaStreamTrack object has just transitioned from the &quot;new&quot; readyState to another state.</td>
<td align="left">16 September 2014 16:46:15</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/states">apis/media capture and streams/MediaStreamTrack/states</a></td>
<td align="left">Returns an object containing all the state variables associated with the allowed constraints.</td>
<td align="left">16 September 2014 16:45:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/stop">apis/media capture and streams/MediaStreamTrack/stop</a></td>
<td align="left">Permanently stop the generation of data for track's source.</td>
<td align="left">16 September 2014 16:44:54</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_capture_and_streams/MediaStreamTrack/unmute">apis/media capture and streams/MediaStreamTrack/unmute</a></td>
<td align="left">This event fires when the MediaStreamTrack object's source is live again after having been temporarily unable to provide data.</td>
<td align="left">16 September 2014 16:43:39</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_capture_and_streams/ended">apis/media capture and streams/ended</a></td>
<td align="left">This event is fired when a MediaStream is stopped.</td>
<td align="left">16 September 2014 16:42:38</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_recorder/MediaRecorder">apis/media recorder/MediaRecorder</a></td>
<td align="left"></td>
<td align="left">15 September 2014 20:24:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_source_extensions/MediaSource/endOfStream">apis/media source extensions/MediaSource/endOfStream</a></td>
<td align="left">Used to indicate that the end of the stream has been reached.</td>
<td align="left">15 September 2014 20:17:27</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/media_source_extensions/VideoPlaybackQuality/creationTime">apis/media source extensions/VideoPlaybackQuality/creationTime</a></td>
<td align="left">Gets the timestamp for when the VideoPlaybackQuality metrics were collected.</td>
<td align="left">15 September 2014 20:15:00</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/media_source_extensions/VideoPlaybackQuality/droppedVideoFrames">apis/media source extensions/VideoPlaybackQuality/droppedVideoFrames</a></td>
<td align="left">Gets the number of dropped video frames.</td>
<td align="left">15 September 2014 20:14:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/localDescription">apis/webrtc/RTCPeerConnection/localDescription</a></td>
<td align="left">Returns the <a href="/apis/webrtc/RTCSessionDescription">RTCSessionDescription</a> most recently passed to the <a href="/apis/webrtc/RTCPeerConnection/setLocalDescription">setLocalDescription()</a> method along with any local candidate descriptions generated since the method was called.</td>
<td align="left">15 September 2014 20:00:55</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/localStreams">apis/webrtc/RTCPeerConnection/localStreams</a></td>
<td align="left">Returns an array of <a href="/apis/webrtc/MediaStream">MediaStream</a> objects added to the connection with <a href="/apis/webrtc/RTCPeerConnection/addStream">addStream()</a>.</td>
<td align="left">15 September 2014 20:00:28</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/negotiationneeded">apis/webrtc/RTCPeerConnection/negotiationneeded</a></td>
<td align="left">The browser anticipates a session negotiation is required. It is triggered whenever <a href="/apis/webrtc/RTCPeerConnection/addStream">addStream</a>, <a href="/apis/webrtc/RTCPeerConnection/removeStream">removeStream</a> or <a href="/apis/webrtc/RTCPeerConnection/setIdentityProvider">setIdentityProvider</a> methods were called successfully and <a href="/apis/webrtc/RTCPeerConnection">RTCPeerConnection</a> signalingState is <code>stable</code> .</td>
<td align="left">15 September 2014 19:59:49</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onaddstream">apis/webrtc/RTCPeerConnection/onaddstream</a></td>
<td align="left">Handles the <a href="/w/index.php?title=apis/webrtc/RTCPeerConnection/addstream&amp;action=edit&amp;redlink=1">addstream</a> event fired when <a href="/apis/webrtc/RTCPeerConnection/setRemoteDescription">setRemoteDescription()</a> is called.</td>
<td align="left">15 September 2014 19:43:06</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/ondatachannel">apis/webrtc/RTCPeerConnection/ondatachannel</a></td>
<td align="left">Handles the <strong>datachannel</strong> event.</td>
<td align="left">15 September 2014 19:42:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/ongatheringchange">apis/webrtc/RTCPeerConnection/ongatheringchange</a></td>
<td align="left">Handles the <strong>gatheringchange</strong> event for a change to the <a href="/apis/webrtc/RTCPeerConnection/iceGatheringState">iceGatheringState</a> property.</td>
<td align="left">15 September 2014 19:41:54</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onicecandidate">apis/webrtc/RTCPeerConnection/onicecandidate</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/icechange">icechange</a> event for a change to the <a href="/apis/webrtc/RTCPeerConnection/iceState">apis/webrtc/RTCPeerConnection/iceState</a> property. It is called any time there is a new ICE candidate added to a previous offer or answer.</td>
<td align="left">15 September 2014 19:40:16</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onicechange">apis/webrtc/RTCPeerConnection/onicechange</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/icechange">icechange</a> event. It is called any time the <a href="/apis/webrtc/RTCPeerConnection/iceState">iceState</a> changes.</td>
<td align="left">15 September 2014 19:39:45</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onidentityresult">apis/webrtc/RTCPeerConnection/onidentityresult</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/identityresult">identityresult</a> event for the success or failure of an identity verification.</td>
<td align="left">15 September 2014 19:39:04</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onnegotiationneeded">apis/webrtc/RTCPeerConnection/onnegotiationneeded</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/negotiationneeded">negotiationneeded</a> event.</td>
<td align="left">15 September 2014 19:38:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onopen">apis/webrtc/RTCPeerConnection/onopen</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/open">open</a> event. Testing.</td>
<td align="left">15 September 2014 19:20:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/onstatechange">apis/webrtc/RTCPeerConnection/onstatechange</a></td>
<td align="left">Handles the <a href="/apis/webrtc/RTCPeerConnection/statechange">statechange</a> event for when the <a href="/apis/webrtc/RTCPeerConnection/readyState">readyState</a> property is changed, i.e. with a call to <a href="/apis/webrtc/RTCPeerConnection/setLocalDescription">setLocalDescription()</a> or <a href="/apis/webrtc/RTCPeerConnection/setRemoteDescription">setRemoteDescription()</a>. The event does not fire when a new RTCPeerConnection object is created.</td>
<td align="left">15 September 2014 19:12:11</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/open">apis/webrtc/RTCPeerConnection/open</a></td>
<td align="left"></td>
<td align="left">12 September 2014 18:31:06</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/readyState">apis/webrtc/RTCPeerConnection/readyState</a></td>
<td align="left">Returns the ready state of the peer connection.</td>
<td align="left">12 September 2014 18:29:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/remoteDescription">apis/webrtc/RTCPeerConnection/remoteDescription</a></td>
<td align="left">Returns the <a href="/apis/webrtc/RTCSessionDescription">RTCSessionDescription</a> most recently passed to the <a href="/apis/webrtc/RTCPeerConnection/setRemoteDescription">setRemoteDescription()</a> method along with any remote candidate descriptions supplied with <a href="/apis/webrtc/RTCPeerConnection/addIceCandidate">addIceCandidate()</a>. Returns null if the remote description has not been set.</td>
<td align="left">12 September 2014 18:28:59</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/remoteStreams">apis/webrtc/RTCPeerConnection/remoteStreams</a></td>
<td align="left">Returns an array of <a href="/apis/webrtc/MediaStream">MediaStream</a> objects added to the connection by the remote peer. This array is updated when the <a href="/apis/webrtc/RTCPeerConnection/onaddstream">addstream</a> and <a href="/apis/webrtc/RTCPeerConnection/removeStream">removestream</a> events are fired.</td>
<td align="left">12 September 2014 18:28:07</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/removeStream">apis/webrtc/RTCPeerConnection/removeStream</a></td>
<td align="left">Removes the given stream from the <a href="/apis/webrtc/RTCPeerConnection/localStreams">localStreams</a> array in the RTCPeerConnection and fires the <a href="/apis/webrtc/RTCPeerConnection/negotiationneeded">negotiationneeded</a> event.</td>
<td align="left">12 September 2014 18:25:44</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/setIdentityProvider">apis/webrtc/RTCPeerConnection/setIdentityProvider</a></td>
<td align="left">Sets the identity provider. Not required if the browser is already configured for an identity provider.</td>
<td align="left">12 September 2014 18:23:15</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/setLocalDescription">apis/webrtc/RTCPeerConnection/setLocalDescription</a></td>
<td align="left">Applies the supplied <a href="/apis/webrtc/RTCSessionDescription">RTCSessionDescription</a> to the local description.</td>
<td align="left">12 September 2014 18:22:21</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/setRemoteDescription">apis/webrtc/RTCPeerConnection/setRemoteDescription</a></td>
<td align="left">Applies the supplied <a href="/apis/webrtc/RTCSessionDescription">RTCSessionDescription</a> to the remote description.</td>
<td align="left">12 September 2014 18:21:40</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/statechange">apis/webrtc/RTCPeerConnection/statechange</a></td>
<td align="left"></td>
<td align="left">12 September 2014 18:20:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/updateIce">apis/webrtc/RTCPeerConnection/updateIce</a></td>
<td align="left">Updates the ICE agent process that gathers local candidates and remote candidates.</td>
<td align="left">12 September 2014 18:19:52</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCSessionDescription/sdp">apis/webrtc/RTCSessionDescription/sdp</a></td>
<td align="left">The string representation of the SDP object.</td>
<td align="left">12 September 2014 18:18:54</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCSessionDescription/type">apis/webrtc/RTCSessionDescription/type</a></td>
<td align="left">The type of SDP object this RTCSessionDescription represents.</td>
<td align="left">12 September 2014 18:18:31</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/websocket/CloseEvent/code">apis/websocket/CloseEvent/code</a></td>
<td align="left">The WebSocket connection close code provided by the server.</td>
<td align="left">12 September 2014 18:07:57</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/websocket/CloseEvent/reason">apis/websocket/CloseEvent/reason</a></td>
<td align="left">Indicates the reason the server closed the WebSocket connection.</td>
<td align="left">12 September 2014 18:07:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/websocket/MessageEvent/data">apis/websocket/MessageEvent/data</a></td>
<td align="left">The data from the server.</td>
<td align="left">12 September 2014 18:05:10</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/websocket/WebSocket/close">apis/websocket/WebSocket/close</a></td>
<td align="left">Closes the WebSocket connection or connection attempt, if any.</td>
<td align="left">12 September 2014 17:21:35</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/websocket/WebSocket/extensions">apis/websocket/WebSocket/extensions</a></td>
<td align="left">The extensions selected by the server.</td>
<td align="left">12 September 2014 17:21:00</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/websocket/WebSocket/protocol">apis/websocket/WebSocket/protocol</a></td>
<td align="left">Indicates the name of the sub-protocol the server selected.</td>
<td align="left">12 September 2014 17:17:44</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/Worker/onerror">apis/workers/Worker/onerror</a></td>
<td align="left">An event listener to be called when an error occurs.</td>
<td align="left">12 September 2014 17:10:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/Worker/onmessage">apis/workers/Worker/onmessage</a></td>
<td align="left">An event listener to be called when a message is received from the worker.</td>
<td align="left">12 September 2014 17:10:20</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/Worker/postMessage">apis/workers/Worker/postMessage</a></td>
<td align="left">Posts a message to the worker with which the object is associated.</td>
<td align="left">12 September 2014 17:09:40</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/Worker/terminate">apis/workers/Worker/terminate</a></td>
<td align="left">Immediately terminates the worker with which the object is associated.</td>
<td align="left">12 September 2014 17:09:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/close">apis/workers/WorkerGlobalScope/close</a></td>
<td align="left">Discards any pending tasks and immediately closes the worker.</td>
<td align="left">12 September 2014 17:07:38</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/importScripts">apis/workers/WorkerGlobalScope/importScripts</a></td>
<td align="left">Fetches one or more script resources, identified by absolute URLs.</td>
<td align="left">12 September 2014 17:06:57</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/location">apis/workers/WorkerGlobalScope/location</a></td>
<td align="left">Returns the WorkerLocation object created for the WorkerGlobalScope object when the worker was created.</td>
<td align="left">12 September 2014 17:06:10</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/navigator">apis/workers/WorkerGlobalScope/navigator</a></td>
<td align="left">Returns an instance of the WorkerNavigator interface, which represents the identity and state of the user agent (the client).</td>
<td align="left">12 September 2014 17:05:17</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/onerror">apis/workers/WorkerGlobalScope/onerror</a></td>
<td align="left">An event listener to be called when an error occurs.</td>
<td align="left">12 September 2014 17:04:39</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/onoffline">apis/workers/WorkerGlobalScope/onoffline</a></td>
<td align="left">An event listener to be called when the worker goes offline.</td>
<td align="left">12 September 2014 17:04:11</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/ononline">apis/workers/WorkerGlobalScope/ononline</a></td>
<td align="left">An event listener to be called when the worker goes online.</td>
<td align="left">12 September 2014 17:03:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/workers/WorkerGlobalScope/self">apis/workers/WorkerGlobalScope/self</a></td>
<td align="left">Returns the WorkerGlobalScope object.</td>
<td align="left">12 September 2014 17:02:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/workers/WorkerLocation/href">apis/workers/WorkerLocation/href</a></td>
<td align="left">Returns the absolute URL that the object represents.</td>
<td align="left">12 September 2014 16:59:33</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/abort-event">apis/xhr/XMLHttpRequest/abort-event</a></td>
<td align="left">When the request has been aborted. For instance, by invoking the abort() method.</td>
<td align="left">11 September 2014 18:44:54</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/error">apis/xhr/XMLHttpRequest/error</a></td>
<td align="left">When the request has failed.</td>
<td align="left">11 September 2014 18:43:20</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/getResponseHeader">apis/xhr/XMLHttpRequest/getResponseHeader</a></td>
<td align="left">Returns the string containing the text of the specified header, or null if the response has not been received or the header does not exist.</td>
<td align="left">11 September 2014 18:40:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/load">apis/xhr/XMLHttpRequest/load</a></td>
<td align="left">When the request has successfully completed.</td>
<td align="left">11 September 2014 18:39:45</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/loadend">apis/xhr/XMLHttpRequest/loadend</a></td>
<td align="left">When the request has completed (either in success or failure).</td>
<td align="left">11 September 2014 18:39:05</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/loadstart">apis/xhr/XMLHttpRequest/loadstart</a></td>
<td align="left">When the request starts.</td>
<td align="left">11 September 2014 18:35:33</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/progress">apis/xhr/XMLHttpRequest/progress</a></td>
<td align="left">While sending and loading data.</td>
<td align="left">11 September 2014 18:32:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/setRequestHeader">apis/xhr/XMLHttpRequest/setRequestHeader</a></td>
<td align="left">Sets the value of an XMLHttpRequest header.</td>
<td align="left">11 September 2014 18:24:52</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/status">apis/xhr/XMLHttpRequest/status</a></td>
<td align="left">Returns the HTTP result code (status) of the response to the request.</td>
<td align="left">11 September 2014 18:24:14</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/xhr/XMLHttpRequest/timeout-event">apis/xhr/XMLHttpRequest/timeout-event</a></td>
<td align="left">When the author specified timeout has passed before the request could complete.</td>
<td align="left">11 September 2014 18:20:09</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/appcache/ApplicationCache/abort">apis/appcache/ApplicationCache/abort</a></td>
<td align="left">Cancels the application cache download process. This method is intended to be used by Web applications showing their own caching progress UI, in case the user wants to stop the update (e.g., because bandwidth is limited).</td>
<td align="left">5 August 2014 17:00:11</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/timing/methods/msWriteProfilerMark">apis/timing/methods/msWriteProfilerMark</a></td>
<td align="left"></td>
<td align="left">7 July 2014 17:57:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/timing/methods/sample">apis/timing/methods/sample</a></td>
<td align="left"></td>
<td align="left">7 July 2014 17:54:35</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/timing/objects/FrameRequestCallback">apis/timing/objects/FrameRequestCallback</a></td>
<td align="left"></td>
<td align="left">7 July 2014 17:50:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/timing/properties/performance">apis/timing/properties/performance</a></td>
<td align="left"></td>
<td align="left">7 July 2014 17:36:14</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/LocalMediaStream/stop">apis/webrtc/LocalMediaStream/stop</a></td>
<td align="left">Permanently halts the generation of data for the tracks' sources and removes the references to the sources.</td>
<td align="left">1 July 2014 23:55:21</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStream/audioTracks">apis/webrtc/MediaStream/audioTracks</a></td>
<td align="left">The MediaStreamTrackList object representing the audio tracks.</td>
<td align="left">1 July 2014 20:39:46</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStream/ended">apis/webrtc/MediaStream/ended</a></td>
<td align="left">True if the ended event has fired on the MediaStream object.</td>
<td align="left">1 July 2014 20:39:18</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStream/label">apis/webrtc/MediaStream/label</a></td>
<td align="left">A globally unique identifier (GUID) of 36 characters that describes the media stream.</td>
<td align="left">1 July 2014 20:38:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStream/onended">apis/webrtc/MediaStream/onended</a></td>
<td align="left">Handles the ended event when fired on the MediaStream object.</td>
<td align="left">1 July 2014 20:37:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStream/videoTracks">apis/webrtc/MediaStream/videoTracks</a></td>
<td align="left">The MediaStreamTrackList object representing the video tracks.</td>
<td align="left">1 July 2014 20:33:14</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack">apis/webrtc/MediaStreamTrack</a></td>
<td align="left">A MediaStreamTrack is one of two kinds, audio or video, and represents the media source, such as a camera.</td>
<td align="left">1 July 2014 19:55:38</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/enabled">apis/webrtc/MediaStreamTrack/enabled</a></td>
<td align="left">True if the track is still associated with its source.</td>
<td align="left">1 July 2014 19:54:50</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/ended">apis/webrtc/MediaStreamTrack/ended</a></td>
<td align="left">The MediaStreamTrack object's source will not provide data; this may be caused by the following:
<ul>
<li>the user has revoked permissions on the application</li>
<li>the source device has been disconnected</li>
<li>the remote peer has stopped sending data</li>
<li>the stop() method was invoked</li>
</ul></td>
<td align="left">1 July 2014 19:54:05</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/kind">apis/webrtc/MediaStreamTrack/kind</a></td>
<td align="left">The value, either <strong>audio</strong> or <strong>video</strong> for the source of the track.</td>
<td align="left">1 July 2014 19:52:42</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/label">apis/webrtc/MediaStreamTrack/label</a></td>
<td align="left">A user agent-assigned string that identifies the track source, as in &quot;internal microphone.&quot;</td>
<td align="left">1 July 2014 19:51:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/muted">apis/webrtc/MediaStreamTrack/muted</a></td>
<td align="left">The MediaStreamTrack object's source is temporarily unable to provide data.</td>
<td align="left">1 July 2014 19:49:39</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/onended">apis/webrtc/MediaStreamTrack/onended</a></td>
<td align="left">Handles the ended event when fired on the MediaStream object.</td>
<td align="left">1 July 2014 19:47:36</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/onmute">apis/webrtc/MediaStreamTrack/onmute</a></td>
<td align="left">Handles the muted event when fired on the MediaStream object.</td>
<td align="left">1 July 2014 19:36:56</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/readyState">apis/webrtc/MediaStreamTrack/readyState</a></td>
<td align="left">The track's ready state; values.</td>
<td align="left">1 July 2014 19:35:58</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrack/unmuted">apis/webrtc/MediaStreamTrack/unmuted</a></td>
<td align="left">The MediaStreamTrack object's source has resumed providing data.</td>
<td align="left">1 July 2014 19:34:44</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList">apis/webrtc/MediaStreamTrackList</a></td>
<td align="left">A MediaStream has two MediaStreamTrackList objects, one for the video tracks and one for the audio tracks.</td>
<td align="left">1 July 2014 19:31:22</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/add">apis/webrtc/MediaStreamTrackList/add</a></td>
<td align="left">Adds a MediaStreamTrack to this track list.</td>
<td align="left">1 July 2014 19:29:51</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/addtrack">apis/webrtc/MediaStreamTrackList/addtrack</a></td>
<td align="left">A MediaStreamTrack has been added to the list.</td>
<td align="left">1 July 2014 19:28:53</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/item">apis/webrtc/MediaStreamTrackList/item</a></td>
<td align="left">Returns the MediaStreamTrack at the specified index value.</td>
<td align="left">1 July 2014 19:28:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/length">apis/webrtc/MediaStreamTrackList/length</a></td>
<td align="left">The number of tracks in the list.</td>
<td align="left">1 July 2014 19:27:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/onaddtrack">apis/webrtc/MediaStreamTrackList/onaddtrack</a></td>
<td align="left">Handles the addtrack event.</td>
<td align="left">1 July 2014 19:27:16</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/onremovetrack">apis/webrtc/MediaStreamTrackList/onremovetrack</a></td>
<td align="left">Handles the removetrack event.</td>
<td align="left">1 July 2014 19:26:46</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/remove">apis/webrtc/MediaStreamTrackList/remove</a></td>
<td align="left">Removes a MediaStreamTrack from this track list.</td>
<td align="left">1 July 2014 19:26:14</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/MediaStreamTrackList/removetrack">apis/webrtc/MediaStreamTrackList/removetrack</a></td>
<td align="left">A MediaStreamTrack has been removed from the list.</td>
<td align="left">1 July 2014 19:25:16</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/binaryType">apis/webrtc/RTCDataChannel/binaryType</a></td>
<td align="left">Returns the value to which it was last set; on creation, must be initialized to the string &quot;blob&quot;.</td>
<td align="left">1 July 2014 18:39:38</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/bufferedAmount">apis/webrtc/RTCDataChannel/bufferedAmount</a></td>
<td align="left">Returns the number of bytes of application data that have been queued using send() but that (as of the last time the event loop started executing a task) have not yet been transmitted to the network.</td>
<td align="left">1 July 2014 18:38:50</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/close">apis/webrtc/RTCDataChannel/close</a></td>
<td align="left">Closes the RTCDataChannel.</td>
<td align="left">1 July 2014 18:34:13</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/label">apis/webrtc/RTCDataChannel/label</a></td>
<td align="left">A unique identifier that can be used to distinguish this RTCDataChannel object from other RTCDataChannel objects.</td>
<td align="left">1 July 2014 18:33:29</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/onclose">apis/webrtc/RTCDataChannel/onclose</a></td>
<td align="left">An event listener to be called when an RTCDataChannel is closed.</td>
<td align="left">1 July 2014 18:32:46</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/onerror">apis/webrtc/RTCDataChannel/onerror</a></td>
<td align="left">An event listener to be called when an error occurs.</td>
<td align="left">1 July 2014 18:31:57</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/onmessage">apis/webrtc/RTCDataChannel/onmessage</a></td>
<td align="left">An event listener to be called when a message is received.</td>
<td align="left">1 July 2014 18:31:26</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/onopen">apis/webrtc/RTCDataChannel/onopen</a></td>
<td align="left">An event listener to be called when an RTCDataChannel is opened.</td>
<td align="left">1 July 2014 18:29:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/readyState">apis/webrtc/RTCDataChannel/readyState</a></td>
<td align="left">Represents the state of the RTCDataChannel object.</td>
<td align="left">1 July 2014 18:27:59</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/reliable">apis/webrtc/RTCDataChannel/reliable</a></td>
<td align="left">Returns true if the RTCDataChannel is reliable, and false otherwise.</td>
<td align="left">1 July 2014 18:25:25</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCDataChannel/send">apis/webrtc/RTCDataChannel/send</a></td>
<td align="left">Sends a message (<em>data</em>) on the RTCDataChannel’s underlying data transport.</td>
<td align="left">1 July 2014 18:23:30</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCIceCandidate">apis/webrtc/RTCIceCandidate</a></td>
<td align="left"></td>
<td align="left">1 July 2014 18:20:13</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection">apis/webrtc/RTCPeerConnection</a></td>
<td align="left">Provides for the connection between remote peers, the transmission of locally generated MediaStream data and arbitrary data between peers.</td>
<td align="left">1 July 2014 18:18:25</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/addIceCandidate">apis/webrtc/RTCPeerConnection/addIceCandidate</a></td>
<td align="left">Provides a remote candidate to the ICE agent.</td>
<td align="left">1 July 2014 18:16:48</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/close">apis/webrtc/RTCPeerConnection/close</a></td>
<td align="left">Closes a peer connection, stops all active ICE processing and any active streaming, and releases any relevant resources such as TURN permissions.</td>
<td align="left">30 June 2014 23:07:33</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/createAnswer">apis/webrtc/RTCPeerConnection/createAnswer</a></td>
<td align="left">Creates a session description compatible with the remote configuration.</td>
<td align="left">30 June 2014 23:06:35</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/createOffer">apis/webrtc/RTCPeerConnection/createOffer</a></td>
<td align="left">Creates a session description compatible with the local configuration.</td>
<td align="left">30 June 2014 23:02:27</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/getIdentityAssertion">apis/webrtc/RTCPeerConnection/getIdentityAssertion</a></td>
<td align="left">Provides an identity assertion.</td>
<td align="left">30 June 2014 23:00:53</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/getStats">apis/webrtc/RTCPeerConnection/getStats</a></td>
<td align="left">Retrieves status information for a given <a href="/apis/webrtc/MediaStreamTrack">MediaStreamTrack</a>.</td>
<td align="left">30 June 2014 23:00:10</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/iceGatheringState">apis/webrtc/RTCPeerConnection/iceGatheringState</a></td>
<td align="left">Returns the gathering state of the ICE agent.</td>
<td align="left">30 June 2014 22:57:11</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/iceState">apis/webrtc/RTCPeerConnection/iceState</a></td>
<td align="left">Returns the ICE state of the ICE agent.</td>
<td align="left">30 June 2014 22:55:30</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/icecandidate">apis/webrtc/RTCPeerConnection/icecandidate</a></td>
<td align="left"></td>
<td align="left">30 June 2014 22:51:46</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/icechange">apis/webrtc/RTCPeerConnection/icechange</a></td>
<td align="left"></td>
<td align="left">30 June 2014 22:51:02</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/quota_management/requestQuota">apis/quota management/requestQuota</a></td>
<td align="left">Requests a new quota for the requesting application.</td>
<td align="left">26 June 2014 00:36:12</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/quota_management/queryUsageAndQuota">apis/quota management/queryUsageAndQuota</a></td>
<td align="left">Queries the current usage (how much data is stored) and quota available for the requesting application.</td>
<td align="left">26 June 2014 00:35:51</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/quota_management/StorageQuota">apis/quota management/StorageQuota</a></td>
<td align="left">Provides a means to query and request storage usage and quota information.</td>
<td align="left">26 June 2014 00:33:58</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/network_information/NetworkInformation/connection">apis/network information/NetworkInformation/connection</a></td>
<td align="left">The object from which connection information is accessed.</td>
<td align="left">25 June 2014 23:38:23</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/network_information/Connection/onchange">apis/network information/Connection/onchange</a></td>
<td align="left">Handles the change event, fired when the Connection changes.</td>
<td align="left">25 June 2014 23:37:17</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/network_information/Connection/metered">apis/network information/Connection/metered</a></td>
<td align="left">A connection is metered when the user's connection is subject to a limitation from his Internet Service Provider strong enough to request web applications to be careful with the bandwidth usage.</td>
<td align="left">25 June 2014 23:36:35</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/network_information/Connection/change">apis/network information/Connection/change</a></td>
<td align="left">Fires when the Connection changes.</td>
<td align="left">25 June 2014 23:35:56</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/network_information/Connection/bandwidth">apis/network information/Connection/bandwidth</a></td>
<td align="left">An estimation of the current bandwidth in MB/s (Megabytes per seconds) available.</td>
<td align="left">25 June 2014 23:35:20</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/network_information/Connection">apis/network information/Connection</a></td>
<td align="left">Provides a handle to the device's connection information.</td>
<td align="left">25 June 2014 23:34:07</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/MediaStream/ended">apis/MediaStream/ended</a></td>
<td align="left">All tracks of the MediaStream object have ended; the MediaStream is said to be finished.</td>
<td align="left">21 June 2014 00:31:06</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/webrtc/RTCPeerConnection/identityresult">apis/webrtc/RTCPeerConnection/identityresult</a></td>
<td align="left"></td>
<td align="left">17 June 2014 13:10:45</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/properties/type">css/media queries/apis/properties/type</a></td>
<td align="left">Gets the media type of the object that displays the <a href="/dom/Document">Document</a> object</td>
<td align="left">17 June 2014 12:02:56</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/media_queries/apis/removeListener">css/media queries/apis/removeListener</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:47:20</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/media">css/media queries/apis/media</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:46:45</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/media_queries/apis/matches">css/media queries/apis/matches</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:46:04</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/matchMedium">css/media queries/apis/matchMedium</a></td>
<td align="left">Indicates whether the document currently matches a media query.</td>
<td align="left">17 June 2014 11:45:01</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/media_queries/apis/matchMedia">css/media queries/apis/matchMedia</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:43:47</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/handleChange">css/media queries/apis/handleChange</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:42:36</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/media_queries/apis/addListener">css/media queries/apis/addListener</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:42:00</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/StyleMedia">css/media queries/apis/StyleMedia</a></td>
<td align="left">A CSS media related functionality and information.</td>
<td align="left">17 June 2014 11:39:13</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/media_queries/apis/MediaQueryListListener">css/media queries/apis/MediaQueryListListener</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:37:56</td>
</tr>
<tr class="even">
<td align="left"><a href="/css/media_queries/apis/MediaQueryList">css/media queries/apis/MediaQueryList</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:36:46</td>
</tr>
<tr class="odd">
<td align="left"><a href="/css/high_contrast_modeapis/properties/ms-high-contrast-adjust">css/high contrast modeapis/properties/ms-high-contrast-adjust</a></td>
<td align="left"></td>
<td align="left">17 June 2014 11:29:14</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/appcache/ApplicationCache/oncached">apis/appcache/ApplicationCache/oncached</a></td>
<td align="left">The resources listed in the manifest have been downloaded, and the application is now cached.</td>
<td align="left">22 June 2013 18:25:04</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/appcache/ApplicationCache/onerror">apis/appcache/ApplicationCache/onerror</a></td>
<td align="left">Indicates an error has occurred.</td>
<td align="left">13 March 2013 19:48:37</td>
</tr>
<tr class="even">
<td align="left"><a href="/apis/appcache/ApplicationCache/ondownloading">apis/appcache/ApplicationCache/ondownloading</a></td>
<td align="left">The user agent has found an update and is fetching it, or is downloading the resources listed by the manifest for the first time.</td>
<td align="left">13 March 2013 19:48:10</td>
</tr>
<tr class="odd">
<td align="left"><a href="/apis/appcache/ApplicationCache/onchecking">apis/appcache/ApplicationCache/onchecking</a></td>
<td align="left">The user agent is checking for an update, or attempting to download the manifest for the first time. This is always the first event in the sequence.</td>
<td align="left">13 March 2013 19:47:38</td>
</tr>
</tbody>
</table>

