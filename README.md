# K
{"content": "var Fyber MraidVideoTracker = function e() {var
r,i,n,t,a,s; let o=!1; try {r Omid SessionClient.default} catch(d) {return FyLogger.log(\e.name "FyberMraidVideoTracker -->init Fyber Omid -> Unable to load OMSDK: \"+d), {} } let
c=r. AdSession, m=r. Partner, 1=r.Context, br. Ad Events, v=r. Media Events; fun ction y (e){\"sessionStart \"=== e.type? (FyLogger.log(\"init FyberOmid -->
FyberMraidVideoTracker
->
sessionStart \"), \ "defined By JavaScript\"===e.data.creativeType&&i.setCr eative Type (\"video\"), \ "defined By JavaScript\"===e.data. impression Type& &i.setImpressionType(\"beginTo Render\"), a. loaded()):\"sessionError\"== = e.type? FyLogger.log(\"initFyber Omid --> FyberMraidVideoTracker -> sessionError:
\"+e):\"session Finish\"===e.type&& (FyberMraid Video Controller. removeEve ntListener(u), FyberMraid Video Controller. remove Video Element ReadyListene r()) } function u(e) { switch (FyLogger.log(\"onEvent --> FyberMraidVideoTracker -> event: \"+e.name), e.name) {case
EVENT VIDEO_START: let
r e. duration; r&& \ "NaN\"!==r|| (r=-1),s.start(r, e.volume); break; case EVENT VIDEO_PAUSE: s.pause(); break; case
EVENT VIDEO_RESUME: s. resume(); break; case
EVENT_VIDEO_COMPLETED:s.complete(); break; case
EVENT VIDEO_VOLUME_CHANGE: s. volume Change (e. volume); break; case EVENT FIRST QUARTILE: s. first Quartile(); break; case
EVENT MIDPOINT: s.midpoint(); break; case
EVENT THIRD QUARTILE: s. third Quartile(); break; case
EVENT VIDEO_BUFFER_START: s.bufferStart(); break; case
EVENT VIDEO_BUFFER FINISH: s. buffer Finish() } } function p(e) e
(e=document.querySelector(\"video\")), t.setVideo Element (e), an
ew b(i), s=new
v(i), i. register SessionObserver (y), FyberMraid Video Controller.registerEv entListener(u), FyberMraidVideo Controller. remove Video Element Ready Listen er(),o&&Fyber MraidVideoTracker.impression() } return {init Omid: function e(r, a) [FyLogger.log(\"initOmid Session --> FyberMraidVideoTracker -> initializing omid session (partner: \"+r+\", version: \"+a+\"}\"), n = new m (r,a), t=new 1(n), i-new c(t); var
s FyberMraid Video Controller. video Element (); s?p(s): Fyber Mraid Video Contr oller.register Video Element ReadyListener(p)}, impression: function
e() {a? (a.impression Occurred (),o= 1) : 0=!0}, adUser Interaction: function e(){s&&s. adUser Interaction (\"click\") } } } ();", "lastModified": "Tue, 19 Mar 2024 07:33:29 GMT"}
