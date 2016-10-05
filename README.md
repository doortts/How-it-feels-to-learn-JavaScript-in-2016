# How-it-feels-to-learn-JavaScript-in-2016

원문: https://hackernoon.com/how-it-feels-to-learn-javascript-in-2016-d3a717dd577f#.x0ic9zicy 

**읽으면서 느낌대로 그대로 타이핑이라 오역/의역 많아요.**

제가 새로 웹 프로젝트를 시작하는데요, 솔직히 최근 몇년간 코딩을 얼마 못했거든요.
세상이 많이 바뀌었다고 들었는데, 당신에 여기서 가장 최근 상황을 잘 아는 엔지니어라고 들었는데 맞죠?

- 음.  네 접니다. 정확히는 프론트 엔드 엔지니어라고 하죠. 2016년에 웹을 하고 있고 비쥬얼라이제이션, 뮤직플레이어, 축구를 할 수 있는 드론등을 하고 있죠. 그리고 얼마전에 JsConf랑 ReactConf 갔다 왔기때문에 웹 앱을 만드는 최신 기술들을 알고 있답니다.

좋아요!! 유저들의 최근 활동을 표시하는 웹 페이지를 만들려고 하고요. 그래서 REST api를 이용해서 데이터를 가져와서 필터링 되는 테이블을 이용해 서버에 변경사항이 있을때마다 화면에 출력하려고요. 제 생각엔 jQuery 이용해서 패치(fetch)해서 데이터를 출력하면 될것같아요

- 오! 맙소사! 이젠 아무도 jQuery 안써요. React 배우세요. 지금은 2016년이라구요

아. 알겠어요. React가 뭐죠?

- 페이스북의 몇몇 사람들이 만든 완전 끝내주는 라이브러리죠. 당신 앱의 성능과 제어권을 보장해주죠. 뷰(view) 변경이 진짜 쉽거든요

그거 좋아보이네요. React 사용하면 서버로부터 데이터를 표시할 수 있는거죠?

- 네. 그런데 우선은 React랑 React DOM을 라이브러리로 웹페이지에 추가해야 해요

잠깐. 왜 라이브러리가 두개죠?

- 그게 하나는 라이브러리고 다른 하나는 JSX로 작성된대로 DOM을 조작하는데 쓰거든요. 

JSX? JSX는 뭐에요?

- JSX는 그냥 자바스크립트 확장인데 XML 비슷하게 생겼어요. DOM 만드는 방법중하나에요. 더 좋은 HTML이라고 생각하면 되요.

HTML에 뭔가 문제가 있나요?

- 지금은 2016년입니다. 누구도 HTML을 직접 작성하는건 안해요

알겠어요. 어쨌든 이 라이브러리 두 개 추가하면 React 쓸 수 있다는 거죠?

- 그렇겐 안되고 Babel을 추가해야 React를 쓸 수 있어요.

라이브러리 하나더요? Babel은 뭐죠?

- 아. Babel은 어떤 자바스크립트 버전을 쓰던 해당 자바스크립트 버전을 쓸수 있게 해주는 트랜스파일러(transpiler)에요. ReactJS 쓰는데 Babel을 추가 안해도 되긴하는데요 그러면 ES5밖에 못쓰게 되는데요, 솔까말 지금은 2016년이잖아요. 다른 잘나가는 개발자들처럼 ES2016+ 로 코딩해야죠. 

ES5? ES2016플러스? 아. 점점 더 모르겠네요... ES5는 뭐고 ES2016+는 뭔가요?

- ES6는 ECMAScript 5를 말하는거에요. 요즘 대부분의 브라우저에서 지원하고 가장 많은 사람들이 사용하는 에디션이죠.

이씨엠에이스크립트?

- 네. 아시다시피 1995년체 최초 릴리즈된 후 1999년에 만들어진 자바스크립트 스크립팅 표준을 말합니다. 95년에는 Livescirpt라고 했었는데 오직 넷스케이브 네비게이터에서만 동작했죠. 그때는 정말 엉망이었죠. 하지만 다행히도 요즘엔 훨씬 좋아졌고 7판(edition)까지 있죠.

7판이라니. 아, 정말..  그럼 ES5랑 ES2016+는 뭐에요?

- 각각 5판이랑 7판을 나타내죠.

잠시만요. 6판은 어디갔어요?

- ES6 말인가요? 음. 그러니까, 각각의 에디션은 이전 에디션의 슈퍼셋이거든요, 그래서 ES2016+ 쓰시면 이전 버전의 모든 기능들을 사용할수 있으세요.

알겠어요. 그럼 왜 ES6 안쓰고 ES2016+ 써요?

- 음.. ES6를 쓸.수.도 있는데요 async라던가 await 라던가 그런 신박한 기능을 쓰려면 ES2016+ 쓰셔야해요. 그렇게 안하면 비동기 호출 흐름제어에 ES6의 제네레이터를 코루틴이랑 같이써서 블럭해야 하거든요.

뭐라는지 하나도 모르겠네요. 단어들도 헷깔리고요. 있잖아요, 그냥 서버에서 데이터 몽땅 가져오면 되는데 CDN으로 jQuery 포함시켜서 AJAX로 하면 안되여?

- 아 진짜. 지금은 2016년이라니까요. 이젠 아무도 jQuery 안써요. 그렇게하면 결국 스파게티 코드로 끝날거라구요. 다들 그걸 잘 알고 있고요

알겠어요. 그럼 앞서 말한 라이브러리 세 개 포함시켜서 데이터 패치해 와서 HTML 테이블에 표시하는 것이 대안이겠네요.

- 음.. 포함시켜야 하긴 하는데 모듈 매니저로 묶어서 하나로 만들어서 해야해요.

아.네. 그런데 모듈 매니저는 뭔가요?

- 무슨환경이냐에 따라 정의가 다르긴 한데요, 웹에서는 보통 AMD나 CommonJS 모듈 지원하는걸 말해요

아...네.. 그럼 AMD랑 CommonJS라는 건...

- 정의에요. 복수개의 자바스크립트 라이브러리와 관심있는 클래스들을 기술하는 방법들이죠. exports랑 requires는 알고 계신거죠? AMD나 CommonJS로 자바스크립트 파일들을 작성하면 Browerify 같은걸로 하나로 묶을 수 있어요.

아하. 대략 이해가 되네요. Browerify는 뭐에요?

- CommonJS로 기술된 의존 파일들을 묶어서 브라우저에서 동작할 수 있게 만들어주는 도굽니다. 대부분의 사람들이 npm 레지스트리에 모듈을 올리기때문에 만들어졌어요.

엠피엠 레지스트리요?

- 아주 큰 공개 저장소에요. 똑똑한 사람들이 코드와 의존 코드들을 모듈로 만들어서 넣어두는 곳이죠.

CDN 같은?

- 그런건 아니고요. 누구나 라이브러리를 올리고 내려받을 수 있는 중앙화된 데이터베이트 같은거라고 보면되요. 개발할때 로컬에서 쓸수도 있고 원한다면 CDN에 올릴수도 있긴하죠.

아하. Bower 같은거구나!

- 네. 그런데 지금은 2016년이랬죠? 요즘은 Bower 아무도 안써요

아. 알겠어요. 그러면 앞서 말한 라이브러리들을 npm에서 내려받아야겠군요.

- 네. React를 쓰시려면 마찬가지로 React 모듈을 내려받아서 작성하신 코드에 import 해야해요. 대부분의 인기있는 자바스크립트 라이브러리를 그런식으로 쓸 수 있어요.

이를테면 Angular 같은?

- 2015년엔 인기모듈이었겠죠. 네. 뭐. Angular도 있을거에요. VueJS나 RxJS나 기타 다른 쿨한 2016년식 라이브러리들도 있을거구요.

우선 React 쓰는걸로 하죠. 이미 알게된게 너무 많아요. 그럼 React를 쓰려면 npm 에서 패치해와서 Browerify 라는걸 사용해서 써야 한다는거죠?

- 네

단순히 의존 모듈 몇 개 묶어서 쓰기엔 너무 복잡해보이네요

- 그렇죠. 그래서 그게 Grunt나 Gulp 나 Broccoli 같은 태스크 매니저를 사용해서 Browerify 실행을 자동화시키는 이유에요. 아맞다! Mimosa를 써도 되구요.

그런트? 걸프? 브로콜리? 미모사? 아놔 뭐에요 이건?

- 태스크 매니저들요. 그런데 사실 요즘엔 좀 그렇고 2015년정도엔 그런걸 썼죠. 그런데 지금은 묶는데 Webpack 써요.

.... 이하 미번역

Makefiles? I thought that was mostly used on C or C++ projects.

-Yeah, but apparently in the web we love making things complicated and then going back to the basics. We do that every year or so, just wait for it, we are going to do assembly in the web in a year or two.

Sigh. You mentioned something called Webpack?

-It’s another module manager for the browser while being kind of a task runner as well. It’s like a better version of Browserify.

Oh, Ok. Why is it better?

-Well, maybe not better, it’s just more opinionated on how your dependencies should be tied. Webpack allows you to use different module managers, and not only CommonJS ones, so for instance native ES6 supported modules.

I’m extremely confused by this whole CommonJS/ES6 thing.

-Everyone is, but you shouldn’t care anymore with SystemJS.

Jesus christ, another noun

-js. Ok, and what is this SystemJS?

-Well, unlike Browserify and Webpack 1.x, SystemJS is a dynamic module loader that allows you to tie multiple modules in multiple files instead of bundling them in one big file.

Wait, but I thought we wanted to build our libraries in one big file and load that!

-Yes, but because HTTP/2 is coming now multiple HTTP requests are actually better.

Wait, so can’t we just add the three original libraries for React??

-Not really. I mean, you could add them as external scripts from a CDN, but you would still need to include Babel then.

Sigh. And that is bad right?

-Yes, you would be including the entire babel-core, and it wouldn’t be efficient for production. On production you need to perform a series of pre-tasks to get your project ready that make the ritual to summon Satan look like a boiled eggs recipe. You need to minify assets, uglify them, inline css above the fold, defer scripts, as well as

I got it, I got it. So if you wouldn’t include the libraries directly in a CDN, how would you do it?

-I would transpile it from Typescript using a Webpack + SystemJS + Babel combo.

Typescript? I thought we were coding in JavaScript!

-Typescript IS JavaScript, or better put, a superset of JavaScript, more specifically JavaScript on version ES6. You know, that sixth version we talked about before?

I thought ES2016+ was already a superset of ES6! WHY we need now this thing called Typescript?

-Oh, because it allows us to use JavaScript as a typed language, and reduce run-time errors. It’s 2016, you should be adding some types to your JavaScript code.

And Typescript obviously does that.

-Flow as well, although it only checks for typing while Typescript is a superset of JavaScript which needs to be compiled.

Sigh… and Flow is?

-It’s a static type checker made by some guys at Facebook. They coded it in OCaml, because functional programming is awesome.

OCaml? Functional programming?

-It’s what the cool kids use nowadays man, you know, 2016? Functional programming? High order functions? Currying? Pure functions?

I have no idea what you just said.

-No one does at the beginning. Look, you just need to know that functional programming is better than OOP and that’s what we should be using in 2016.

Wait, I learned OOP in college, I thought that was good?

-So was Java before being bought by Oracle. I mean, OOP was good back in the days, and it still has its uses today, but now everyone is realising modifying states is equivalent to kicking babies, so now everyone is moving to immutable objects and functional programming. Haskell guys had been calling it for years, 

-and don’t get me started with the Elm guys

- but luckily in the web now we have libraries like Ramda that allow us to use functional programming in plain JavaScript.
Are you just dropping names for the sake of it? What the hell is Ramnda?

-No. Ramda. Like Lambda. You know, that David Chambers’ library?

David who?

-David Chambers. Cool guy. Plays a mean Coup game. One of the contributors for Ramda. You should also check Erik Meijer if you are serious about learning functional programming.

And Erik Meijer is…?

-Functional programming guy as well. Awesome guy. He has a bunch of presentations where he trashes Agile while using this weird coloured shirt. You should also check some of the stuff from Tj, Jash Kenas, Sindre Sorhus, Paul Irish, Addy Osmani-

Ok. I’m going to stop you there. All that is good and fine, but I think all that is just so complicated and unnecessary for just fetching data and displaying it. I’m pretty sure I don’t need to know these people or learn all those things to create a table with dynamic data. Let’s get back to React. How can I fetch the data from the server with React?

-Well, you actually don’t fetch the data with React, you just display the data with React.

Oh, damn me. So what do you use to fetch the data?

-You use Fetch to fetch the data from the server.

I’m sorry? You use Fetch to fetch the data? Whoever is naming those things needs a thesaurus.

-I know right? Fetch it’s the name of the native implementation for performing XMLHttpRequests against a server.

Oh, so AJAX.

-AJAX is just the use of XMLHttpRequests. But sure. Fetch allows you to do AJAX based in promises, which then you can resolve to avoid the callback hell.

Callback hell?

-Yeah. Every time you perform an asynchronous request against the server, you need to wait for its response, which then makes you to add a function within a function, which is called the callback pyramid from hell.

Oh, Ok. And this promise thing solves it?

-Indeed. By manipulating your callbacks through promises, you can write easier to understand code, mock and test them, as well as perform simultaneous requests at once and wait until all of them are loaded.

And that can be done with Fetch?

-Yes, but only if your user uses an evergreen browser, otherwise you need to include a Fetch polyfill or use Request, Bluebird or Axios.

How many libraries do I need to know for god’s sake? How many are of them?

-It’s JavaScript. There has to be thousands of libraries that all do the same thing. We know libraries, in fact, we have the best libraries. Our libraries are huuuge, and sometimes we include pictures of Guy Fieri in them.

Did you just say Guy Fieri? Let’s get this over with. What these Bluebird, Request, Axios libraries do?

-They are libraries to perform XMLHttpRequests that return promises.

Didn’t jQuery’s AJAX method start to return promises as well?

-We don’t use the “J” word in 2016 anymore. Just use Fetch, and polyfill it when it’s not in a browser or use Bluebird, Request or Axios instead. Then manage the promise with await within an async function and boom, you have proper control flow.

It’s the third time you mention await but I have no idea what it is.

-Await allows you to block an asynchronous call, allowing you to have better control on when the data is being fetch and overall increasing code readability. It’s awesome, you just need to make sure you add the stage-3 preset in Babel, or use syntax-async-functions and transform-async-to-generator plugin.

This is insane.

-No, insane is the fact you need to precompile Typescript code and then transpile it with Babel to use await.

Wat? It’s not included in Typescript?

-It does in the next version, but as of version 1.7 it only targets ES6, so if you want to use await in the browser, first you need to compile your Typescript code targeting ES6 and then Babel that shit up to target ES5.

At this point I don’t know what to say.

-Look, it’s easy. Code everything in Typescript. All modules that use Fetch compile them to target ES6, transpile them with Babel on a stage-3 preset, and load them with SystemJS. If you don’t have Fetch, polyfill it, or use Bluebird, Request or Axios, and handle all your promises with await.

We have very different definitions of easy. So, with that ritual I finally fetched the data and now I can display it with React right?

-Is your application going to handle any state changes?

Err, I don’t think so. I just need to display the data.

-Oh, thank god. Otherwise I would had to explain you Flux, and implementations like Flummox, Alt, Fluxible. Although to be honest you should be using Redux.

I’m going to just fly over those names. Again, I just need to display data.

-Oh, if you are just displaying the data you didn’t need React to begin with. You would had been fine with a templating engine.

Are you kidding me? Do you think this is funny? Is that how you treat your loved ones?

-I was just explaining what you could use.

Stop. Just stop.

-I mean, even if it’s just using templating engine, I would still use a Typescript + SystemJS + Babel combo if I were you.

I need to display data on a page, not perform Sub Zero’s original MK fatality. Just tell me what templating engine to use and I’ll take it from there.

-There’s a lot, which one you are familiar with?

Ugh, can’t remember the name. It was a long time ago.

-jTemplates? jQote? PURE?

Err, doesn’t ring a bell. Another one?

-Transparency? JSRender? MarkupJS? KnockoutJS? That one had two-way binding.

Another one?

-PlatesJS? jQuery-tmpl? Handlebars? Some people still use it.

Maybe. Are there similar to that last one?

-Mustache, underscore? I think now even lodash has one to be honest, but those are kind of 2014.

Err.. maybe it was newer.

-Jade? DustJS?

No.

-DotJS? EJS?

No.

-Nunjucks? ECT?

No.

-Mah, no one likes Coffeescript syntax anyway. Jade?

No, you already said Jade.

-I meant Pug. I meant Jade. I mean, Jade is now Pug.

Sigh. No. Can’t remember. Which one would you use?

-Probably just ES6 native template strings.

Let me guess. And that requires ES6.

-Correct.

Which, depending on what browser I’m using needs Babel.

-Correct.

Which, if I want to include without adding the entire core library, I need to load it as a module from npm.

-Correct.

Which, requires Browserify, or Wepback, or most likely that other thing called SystemJS.

-Correct.

Which, unless it’s Webpack, ideally should be managed by a task runner.

-Correct.

But, since I should be using functional programming and typed languages I first need to pre-compile Typescript or add this Flow thingy.

-Correct.

And then send that to Babel if I want to use await.

-Correct.

So I can then use Fetch, promises, and control flow and all that magic.

-Just don’t forget to polyfill Fetch if it’s not supported, Safari still can’t handle it.

You know what. I think we are done here. Actually, I think I’m done. I’m done with the web, I’m done with JavaScript altogether.

-That’s fine, in a few years we all are going to be coding in Elm or WebAssembly.

I’m just going to move back to the backend. I just can’t handle these many changes and versions and editions and compilers and transpilers. The JavaScript community is insane if it thinks anyone can keep up with this.

-I hear you. You should try the Python community then.

Why?

-Ever heard of Python 3?
