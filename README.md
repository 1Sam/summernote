# summernote
[에디터 스킨] 섬머노트


xe/modules/editor/skins/summernote/


참고 : http://summernote.org/#/features


<pre>
<!--@foreach(Context::getJsFile() as $key => $jsfile)-->

	<!--@if(preg_match('/jquery.prettyPhoto.js/i',$jsfile['file']))-->{@$ptyptojs='Y'}<!--@end-->

<!--@end-->

<load cond="$ptyptojs != 'Y'" target="jquery.prettyPhoto.js" />




만약 이전에 로딩한 js파일을 삭제하고 새로운 js파일을 로딩하려면

{@$ptyptojs='Y'} 을

{@Context::unloadJsFile($jsfile['file'])} 

으로 수정하고

<load cond="$ptyptojs != 'Y'" target="jquery.prettyPhoto.js" /> 을

<load target="jquery.prettyPhoto.js" />

으로 수정하면 됩니다. </pre>
