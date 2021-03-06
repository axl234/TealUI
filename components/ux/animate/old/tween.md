<article class="demo"><script>var tween = new Fx.Tween(); Demo.writeExamples({ 'Fx.Tween#run(100)': function () { return tween.run({ elem: Dom.get('a'), params: { width: 100 } }); }, 'Fx.Tween#run("100")': function () { return tween.run({ elem: Dom.get('a'), params: { width: "100" } }); }, 'Fx.Tween#run("+=10")': function () { return tween.run({ elem: Dom.get('a'), params: { width: '+=10' } }); }, 'Fx.Tween#run("-=10")': function () { return tween.run({ elem: Dom.get('a'), params: { width: '-=10' } }); }, 'Fx.Tween#run("0-100")': function () { return tween.run({ elem: Dom.get('a'), params: { width: "0-100" } }); } }, { times: 8 });</script></article>

<article class="demo">

<div id="all">

<div id="a" class="a">id=a margin=30 padding=8

<div id="b" class="b" _tag="b">id=b padding=8

<div id="c" class="c">id=c border=1 margin=4 auto width=300</div>

</div>

<div id="d" class="d">id=d border=10 padding=8</div>

</div>

</div>

<script>var a = Dom.get('a'), b = Dom.get('b'), c = Dom.get('c'), d = Dom.get('d'), o = Dom.get('o'), abcd = new Dom(Dom.get('all').getElementsByTagName("div")); Demo.writeExamples({ 'Animate': '-', 'createAnimate': function () { new Fx.Tween().run({ elem: a, params: { height: 500 } }).run({ elem: a, params: { height: 200 } }).run({ elem: a, params: { height: 100 } }) }, 'animateHeight': 'Dom.animate(d, {height: 500});Dom.animate(d,{height: 100});Dom.animate(d,{height: 30})', 'animateOpacity': 'Dom.animate(a,{opacity: 0});Dom.animate(a,{opacity: 1}); Dom.animate(a,{opacity: 0}); Dom.animate(a,{opacity: 1})', 'animateScrollTop': 'Dom.animate(document, {scrollTop: 400})', 'animateBackgroundColor': 'Dom.animate(a,{"background-color": "#efefef"})', 'Toggle': '-', 'toggle': 'Dom.toggle(a,1000)', 'toggleHeight': 'Dom.toggle(a,{effect:"height", duration:1000})', 'toggleWidth': 'Dom.toggle(a,{effect:"width", duration:1000})', 'toggleAll': 'Dom.toggle(a,{effect:"all", duration:1000})', 'toggleLeft': 'Dom.toggle(a,{effect:"left", duration:1000})', 'toggleTop': 'Dom.toggle(a,{effect:"top", duration:1000})', 'toggleRight': 'Dom.toggle(a,{effect:"right", duration:1000})', 'toggleBottom': 'Dom.toggle(a,{effect:"bottom", duration:1000})', 'hide(1000)': 'Dom.hide(a,1000)', 'hide': 'Dom.hide(a,1);' }, { times: 8 });</script></article>

<article class="demo">

> 本组件是 Tween 的扩展。它让 Tween 支持处理颜色的渐变值。

<script>var tween = new Fx.Tween(); Demo.writeExamples({ 'Fx.Tween#run(#000000)': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: '#000000' } }); }, 'Fx.Tween#run(rgb(0, 0, 0))': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: 'rgb(0, 0, 0)' } }); }, 'Fx.Tween#run("#000000-#ffffff")': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: '#000000-#ffffff' } }); } }, { times: 8 });</script></article>

<article class="demo">

> 本组件是 Color 的扩展。它让 Color 支持识别系统内置颜色。

<script>var tween = new Fx.Tween(); Demo.writeExamples({ 'Fx.Tween#run(green-blue)': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: 'green-blue' } }); } }, { times: 8 });</script></article>

<article class="demo">

> 本组件是 Tween 的扩展。它让 Tween 支持处理颜色的渐变值。

<script>var tween = new Fx.Tween(); Demo.writeExamples({ 'Fx.Tween#run(#000000)': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: '#000000' } }); }, 'Fx.Tween#run(rgb(0, 0, 0))': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: 'rgb(0, 0, 0)' } }); }, 'Fx.Tween#run("#000000-#ffffff")': function () { return tween.run({ elem: Dom.get('a'), params: { backgroundColor: '#000000-#ffffff' } }); } }, { times: 8 });</script></article>

# 类Flash的渐变特效


        #a {
            background: #DCDCDC;
            margin: 30px;
            padding: 8px;
        }

        #b {
            background: #EDEDED;
            padding: 8px;
        }

        #c {
            background: #EAF2F5;
            border: 1px solid #ffffff;
            margin: 4px auto;
            width: 300px;
            text-align: center;
        }

        #d {
            background: #EAF2F5;
            border: 10px solid #BEDCE7;
            padding: 8px;
        }

            var tween = new Fx.Tween();
            Demo.writeExamples({
                'Fx.Tween#run(100)': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            width: 100
                        }
                    });
                },
                'Fx.Tween#run("100")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            width: "100"
                        }
                    });
                },
                'Fx.Tween#run("+=10")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            width: '+=10'
                        }
                    });
                },
                'Fx.Tween#run("-=10")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            width: '-=10'
                        }
                    });
                },
                'Fx.Tween#run("0-100")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            width: "0-100"
                        }
                    });
                }
            }, { times: 8 });

                id=a margin=30 padding=8

                    id=b padding=8
                    id=c border=1 margin=4 auto width=300

                id=d border=10 padding=8

            var a = Dom.get('a'), b = Dom.get('b'), c = Dom.get('c'), d = Dom.get('d'), o = Dom.get('o'), abcd = new Dom(Dom.get('all').getElementsByTagName("div"));

            Demo.writeExamples({
                'Animate': '-',
                'createAnimate': function () {
                    new Fx.Tween().run({
                        elem: a,
                        params: { height: 500 }
                    }).run({
                        elem: a,
                        params: { height: 200 }
                    }).run({
                        elem: a,
                        params: { height: 100 }
                    })

                },
                'animateHeight': 'Dom.animate(d, {height: 500});Dom.animate(d,{height: 100});Dom.animate(d,{height: 30})',
                'animateOpacity': 'Dom.animate(a,{opacity: 0});Dom.animate(a,{opacity: 1}); Dom.animate(a,{opacity: 0}); Dom.animate(a,{opacity: 1})',
                'animateScrollTop': 'Dom.animate(document, {scrollTop: 400})',
                'animateBackgroundColor': 'Dom.animate(a,{"background-color": "#efefef"})',
                'Toggle': '-',
                'toggle': 'Dom.toggle(a,1000)',
                'toggleHeight': 'Dom.toggle(a,{effect:"height", duration:1000})',
                'toggleWidth': 'Dom.toggle(a,{effect:"width", duration:1000})',
                'toggleAll': 'Dom.toggle(a,{effect:"all", duration:1000})',
                'toggleLeft': 'Dom.toggle(a,{effect:"left", duration:1000})',
                'toggleTop': 'Dom.toggle(a,{effect:"top", duration:1000})',
                'toggleRight': 'Dom.toggle(a,{effect:"right", duration:1000})',
                'toggleBottom': 'Dom.toggle(a,{effect:"bottom", duration:1000})',
                'hide(1000)': 'Dom.hide(a,1000)',
                'hide': 'Dom.hide(a,1);'
            }, { times: 8 });

        本组件是 Tween 的扩展。它让 Tween 支持处理颜色的渐变值。

            var tween = new Fx.Tween();
            Demo.writeExamples({
                'Fx.Tween#run(#000000)': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: '#000000'
                        }
                    });
                },
                'Fx.Tween#run(rgb(0, 0, 0))': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: 'rgb(0, 0, 0)'
                        }
                    });
                },
                'Fx.Tween#run("#000000-#ffffff")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: '#000000-#ffffff'
                        }
                    });
                }
            }, { times: 8 });

        本组件是 Color 的扩展。它让 Color 支持识别系统内置颜色。

            var tween = new Fx.Tween();
            Demo.writeExamples({
                'Fx.Tween#run(green-blue)': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: 'green-blue'
                        }
                    });
                }
            }, { times: 8 });

        本组件是 Tween 的扩展。它让 Tween 支持处理颜色的渐变值。

            var tween = new Fx.Tween();
            Demo.writeExamples({
                'Fx.Tween#run(#000000)': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: '#000000'
                        }
                    });
                },
                'Fx.Tween#run(rgb(0, 0, 0))': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: 'rgb(0, 0, 0)'
                        }
                    });
                },
                'Fx.Tween#run("#000000-#ffffff")': function () {
                    return tween.run({
                        elem: Dom.get('a'),
                        params: {
                            backgroundColor: '#000000-#ffffff'
                        }
                    });
                }
            }, { times: 8 });
