<header id="header">[返回](javascript:history.back();) header</header>

<section id="body">

<div class="x-page">

<menu>*   [页面 1: helle world](index.html)*   [页面 2: 使用 App.ready() 初始化页面](subpage-2.html)*   [页面 3: 使用 <script> 加载业务代码](subpage-3.html)*   [页面 4: 使用 startLoading() 异步加载页面](subpage-4.html)*   [页面 5: 使用 App.go() 在页面间传参](subpage-5.html)*   [页面 6: 使用 App.go() 在页面间跳转](subpage-6.html)*   [页面 7: 使用页面的 hide 和 show 事件](subpage-7.html)</menu>

<input type="text" id="input"> <input type="button" id="button" value="按我"> <script>App.ready(function (page) { // 如果向当前页面传递了参数，则设置。 if (page.params.value) { page.find('#input').val(page.params.value); } page.find('#button').click(function () { App.go('subpage-6.html', { value: page.find('#input').val() }); }); });</script> </div>

</section>

<footer id="footer">footer</footer>