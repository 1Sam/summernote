# summernote
[에디터 스킨] 섬머노트


xe/modules/editor/skins/summernote/


참고 : http://summernote.org/#/features


<pre>
<p>&lt;<a href="mailto:!--@foreach(Context::getJsFile">!--@foreach(Context::getJsFile</a>() as $key =&gt; $jsfile)--&gt;</p>
<p>&nbsp;&lt;<a href="mailto:!--@if(preg_match('/jquery.prettyPhoto.js/i',$jsfile['file']))-->{@$ptyptojs='Y'}<!--@end">!--@if(preg_match('/jquery.prettyPhoto.js/i',$jsfile['file']))--&gt;{@$ptyptojs='Y'}&lt;!--@end</a>--&gt;</p>
<p>&lt;<a href="mailto:!--@end">!--@end</a>--&gt;</p>
<p>&lt;load cond="$ptyptojs != 'Y'" target="jquery.prettyPhoto.js" /&gt;</p>
<p><br></p>
<p><br>만약 이전에 로딩한 js파일을 삭제하고 새로운 js파일을 로딩하려면</p>
<p><a href="mailto:{@$ptyptojs='Y'">{@$ptyptojs='Y'</a>} 을</p>
<p><a href="mailto:{@Context::unloadJsFile($jsfile['file'">{@Context::unloadJsFile($jsfile['file'</a>])} </p>
<p>으로 수정하고</p>
<p>&lt;load cond="$ptyptojs != 'Y'" target="jquery.prettyPhoto.js" /&gt; 을</p>
<p>&lt;load target="jquery.prettyPhoto.js" /&gt;</p>
<p>으로 수정하면 됩니다. </p> </pre>
