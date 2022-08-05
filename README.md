
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
        <title>无锋剑客的博客_集群,redis,云平台,自动化运维,Web服务器,MongoDB,Docker,Kubernetes、Helm,Linux,Iaas，Paas，Caas_51CTO博客</title>
    <meta name="keywords" content="无锋剑客的博客,集群,redis,云平台,自动化运维,Web服务器,MongoDB,Docker,Kubernetes、Helm,Linux,Iaas，Paas，Caas,技术博客,51CTO博客">
<meta name="description" content="无锋剑客的博客，集群,redis,云平台,自动化运维,Web服务器,MongoDB,Docker,Kubernetes、Helm,Linux,Iaas，Paas，Caasit技术文章。">    <meta name="applicable-device" content="pc">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta http-equiv="Cache-Control" content="no-siteapp" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge,chrome=1" />
    <meta name="msvalidate.01" content="91C5324FE68C0A46FA65F3FEC225EA65" />
    <link rel="canonical" href="https://blog.51cto.com/michaelkang">
    <link type="favicon" rel="shortcut icon" href="/favicon.ico" />
        <link href="https://static2.51cto.com/edu/blog/css/base.css?v=0d989611f8" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/blog-static/css/header.css?v=f5fb294b94" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/css/other.css?v=0228d642b1" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/css/list_tab.css?v=ff54e0fbe7" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/blog-static/iconFont/iconfont.css?v=2f2311118b" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/cto/font/fontface.css?v=c21cfdd5a7" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/blog-static/css/newbloger/bloger.css?v=a5051fb551" rel="stylesheet"><link href="https://static2.51cto.com/edu/blog/scss/common/medal.css?v=6baad06a01" rel="stylesheet">    <script src="//aeu.alicdn.com/waf/antidomxss_v640.js"></script><script src="//aeu.alicdn.com/waf/interfaceacting211222.js"></script><script>var userId=""</script>
    <script async src="https://static2.51cto.com/edu/blog/js/googletagmanager.js"></script>
    <script>
        var HOME_URL = 'https://home.51cto.com/';
        var STATICPATH = 'https://static2.51cto.com/edu/';
        var SA_SERVER_URL_YM = 'https://sc.51cto.com/sa?project=production';
    </script>
    <script src="https://static2.51cto.com/edu/center/js/jquery.min.js"></script><script src="https://static2.51cto.com/edu/center/js/interaction_iframe.js"></script><script src="https://static2.51cto.com/edu/blog/js/jquery.cookie.js?v=d5528dde00"></script><script src="https://static2.51cto.com/edu/blog/js/cookie.js?v=89fd444508"></script><script src="https://static2.51cto.com/edu/blog/js/login.js?v=8ec8d7c738"></script><script src="https://static2.51cto.com/edu/blog/blog-static/js/common.js?v=e6889804a7"></script><script src="https://static2.51cto.com/edu/blog/js/mbox.js?v=aa29b768eb"></script><script src="https://static2.51cto.com/edu/blog/js/follow.js?v=807b32440c"></script><script src="https://static2.51cto.com/edu/blog/js/vip.js?v=38c6367219"></script><script src="https://static2.51cto.com/edu/blog/js/moment.min.js?v=0e7067c46a"></script><script src="https://static2.51cto.com/edu/blog/blog-static/js/webp.js?v=fcd5c0087e"></script></head>
<script src="https://static2.51cto.com/edu/blog/js/statisticsdb.js?v=1.0.2" charset="utf-8"></script>
<script src="https://static2.51cto.com/edu/blog/blog-static/js/shence.js?v=2.0.5" charset="utf-8"></script>
<body>
<img src="https://static2.51cto.com/edu/blog/mobile/images/share_default.jpg" border="0" style="width:0; height:0; position:absolute;">
  <!--[if lt IE 9]>
  <script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script>
  <script src="https://oss.maxcdn.com/libs/respond.js/1.3.0/respond.min.js"></script>
<![endif]-->
<header class="home-top">
    <div class="Page">
        <div class="top-box">
            <div class="item-lf"><a class="top" href="https://www.51cto.com/" target="_blank"  rel="nofollow">51CTO首页</a></div>
             <div class="item-lf">
                <a href="https://www.51cto.com/dev?utm_source=hometop" target="_blank">内容精选</a>
            </div>
            <div class="item-lf">
                <a href="https://blog.51cto.com/" target="_blank">博客</a>
            </div>
            <div class="item-lf">
                <a class="subweb" href="https://edu.51cto.com?utm_source=hometop" data-id="2" target="_blank"  rel="nofollow">学堂</a>
            </div>
            <div class="item-lf">
                <a class="subweb" href="https://e.51cto.com/?utm_platform=pc&amp;utm_medi-um=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar" data-id="3" target="_blank" rel="nofollow">精培</a>
            </div>
            <div class="item-lf">
                <a class="subweb" href="https://b.51cto.com/index?utm_source=hometop" data-id="4" target="_blank" rel="nofollow">企业培训</a>
            </div>
            <div class="item-lf">
                <a class="subweb" href="https://x.51cto.com/?www" data-id="5" target="_blank" rel="nofollow">CTO训练营</a>
            </div>
            <div class="item-lf">
                <a class="subweb" href="https://ost.51cto.com/openharmony?utm_source=hometop" data-id="6" target="_blank" rel="nofollow">开源基础软件社区</a>
            </div>
            <div class="item-lf">
                <a href="https://metacon.51cto.com?utm_source=blogtop" target="_blank" rel="nofollow">元宇宙大会</a>
            </div>
            <div class="item-lf hot">
                <a
                    class="top"
                    href="https://aisummit.51cto.com/?utm_source=wwwtop"
                    target="_blank"
                >AISummit人工智能大会</a>
                <div class="hot-div">
                    <img src="https://s1.51cto.com/images/100/media/hot.png" alt="">
                </div>
            </div>
            <div class="top-right">
                <div class="item-rt"><span class="subweb" data-id="8">移动端</span></div>
                <div class="item-rt"><span class="subweb" data-id="7">公众号矩阵</span></div>
                <div class="item-rt"><a href="http://so.51cto.com/?keywords=&amp;sort=time" target="_blank" class="search-top" rel="nofollow"><i class="iconblog blogsou blog-search"></i></a></div>
            </div>
        </div>
    </div>
    <div class="nav-more-container" style="height: 0px;">
        <div class="Page nav-contant-box" style="height: 0px; z-index: 0;">
            <div class="nav-contant nav-contant1" data-id="1" style="height: 0px; z-index: 0;">
                <a href="https://blog.51cto.com/" target="_blank">博客</a>
            </div>
            <div class="nav-contant nav-contant2" data-id="2" style="height: 0px; z-index: 0;">
                <a href="https://edu.51cto.com/courselist/index-zh5.html?utm_source=hometop" target="_blank" rel="nofollow">免费课程</a>
                <a href="https://edu.51cto.com/ranking/index.html?utm_source=hometop" target="_blank" rel="nofollow">课程排行</a>
                <a href="https://e.51cto.com/ncamp/list?utm_platform=pc&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=13" target="_blank" rel="nofollow">直播课</a>
                <a href="https://e.51cto.com/rk/?utm_platform=pc&amp;utm_medi-um=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=14" target="_blank" rel="nofollow">软考学堂</a>
            </div>
            <div class="nav-contant nav-contant3" data-id="3" style="height: 0px; z-index: 0;">
                <a href="https://e.51cto.com/?utm_platform=pc&amp;utm_medi-um=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar" target="_blank" rel="nofollow">精品班</a>
                <a href="https://e.51cto.com/wejob/list?pid=5&amp;utm_platform=pc&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=41" target="_blank" rel="nofollow">厂商认证</a>
                <a href="https://e.51cto.com/wejob/list?pid=1&amp;utm_platform=pc&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=42" target="_blank" rel="nofollow">IT技术</a>
                <a href="https://e.51cto.com/rk/?utm_platform=pc&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_xyzq_rightwzl&amp;rtm_frd=07&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=43" target="_blank" rel="nofollow">2022年软考</a>
                <a href="https://e.51cto.com/wejob/list?pid=33&amp;utm_platform=pc&amp;utm_medium=51cto&amp;utm_source=zhuzhan&amp;utm_content=sy_topbar&amp;rtm_frd=44" target="_blank" rel="nofollow">PMP项目管理</a>
            </div>
            <div class="nav-contant nav-contant4" data-id="4" style="height: 0px; z-index: 0;">
                <a href="https://b.51cto.com/index?utm_source=hometop" target="_blank" rel="nofollow">在线学习</a>
                <a href="https://b.edu.51cto.com/site/home" target="_blank" rel="nofollow">企业服务</a>
            </div>
            <div class="nav-contant nav-contant5" data-id="5" style="height: 0px; z-index: 0;">
                <a href="https://x.51cto.com/?www" target="_blank" rel="nofollow">CTO训练营</a>
                <a href="https://x.51cto.com/act/cto/tl" target="_blank" rel="nofollow">技术经理研习营</a>
                <a href="https://x.51cto.com/act/cto/leatech2021?www1" target="_blank" rel="nofollow">LeaTech峰会</a>
            </div>
            <div class="nav-contant nav-contant6" data-id="6" style="height: 0px; z-index: 0;">
                <a href="https://ost.51cto.com/postlist" target="_blank" rel="nofollow">文章</a>
                <a href="https://ost.51cto.com/resource" target="_blank" rel="nofollow">资源</a>
                <a href="https://ost.51cto.com/answerlist" target="_blank" rel="nofollow">问答</a>
                <a href="https://ost.51cto.com/study" target="_blank" rel="nofollow">开源课堂</a>
                <a href="https://ost.51cto.com/column" target="_blank" rel="nofollow">专栏</a>
                <a href="https://ost.51cto.com/activity" target="_blank" rel="nofollow">直播</a>
            </div>
            <div class="nav-contant nav-contant7" data-id="7" style="height: 0px; z-index: 0;"></div>
            <div class="nav-contant nav-contant8" data-id="8" style="height: 0px; z-index: 0;"></div>
        </div>
    </div>
</header>
<div class="Header" style="height:61px;">
  <div class="Page clearfix ">
      <div class="Logo"><a href="https://blog.51cto.com/"><img src="https://static2.51cto.com/edu/blog/images/logonew5.png" alt="51CTO博客" width="202" title="51CTO博客"><h2>51CTO博客</h2></a></div>
      <ul class="Navigates fl commonhide">
      <li ><a href="https://blog.51cto.com/">首页</a>
        <div class="spam-classifications" style="display:none;">
          <div class="spam-classifications-content">
          <div class="classification-ipc"  id="classification-ipc"></div> <div class="classification-primary-list-box" id="classification-primary-list-box"></div>

          </div>
        </div>
      </li>
      <li ><a href="https://blog.51cto.com/nav/following">关注</a></li>
        <li ><a href="https://blog.51cto.com/ranking">热榜</a></li>
      <li class="">
        <a  href="https://blog.51cto.com/cloumn/index" target="_blank">订阅专栏</a>
      </li>
      
                  </ul>
    <ul class="Navigates Navigates-right fr">
      <li class="more maps  ">
        <a href="javascript:void(0);" class="menu iconblog bloggengduo"></a>
        <div>
          <div class="ins">

            <a href="https://edu.51cto.com/" target="_blank">学堂</a>
            <a href="https://e.51cto.com/" target="_blank" rel="nofollow">精培</a>
            <a href="https://ost.51cto.com/?utm_source=blognav" target="_blank">开源社区</a>
            <a href="http://x.51cto.com" target="_blank" rel="nofollow">CTO训练营</a>
            <a href="http://www.51cto.com" target="_blank">51CTO</a>
              <a href="https://blog.51cto.com/class-blog/index" target="_blank">班级博客</a>
          </div>
        </div>
      </li>
              <li class="logins">
			    <a href="https://home.51cto.com/index?from_service=blog&scene=login1&reback=https://blog.51cto.com/michaelkang" target="_self" class="clearfix" rel="nofollow" ><span class="fl">登录</span><b class="fgline fl"></b><span class="fl">注册</span></a>
        </li>
                        <li class="mRead commonhide">
            <a href="javascript:;" rel="nofollow"> <u></u></a>
            <div>
              <div class="ins">
                  <div class="towD-box">
                      <img  id="towD-box1">
                      <p>手机随时阅读</p>
                  </div>
                  <div class="towD-box">
                      <img  id="towD-box2">
                      <p>新人专享大礼包￥24</p>
                  </div>
                </div>
            </div>
        </li>
                  <li class="write commonhide"><a href="javascript:;" id="toPublish" onClick="Login({scene:'write1'})" rel="nofollow"> <span ></span>写文章</a></li>
                <li class="search commonhide">

          <form class="fr form-search" method='get' action="https://blog.51cto.com/search/result" target="_blank">
            <input type="text" name="q"  placeholder="大家都在搜索..." id="TopSearchInput" autocomplete="off">
            <button  class="iconblog blogsou" id="TopSearchBtn"></button>
          </form>
                    <div class="focusSelect focusSelect_his">

              <div class="searchHistoryList">
                <div class="clearfix hishead">搜索历史
                  <span class="clearhis"><i class="iconblog blogshanchu18 "></i>清空</span>
                </div>
                <div class="hisitem-wrap"></div>
              </div>

              <div class="hotList">
                <div class="clearfix hishead">热门搜索</div>
                <div class="hot-wrap"></div>
              </div>

          </div>

          <div class="focusSelect focusSelect_key" >
            <div class="keyitem-wrap">

            </div>
            <div class="clearfix checkSearchResult">
              <span>查看【</span>
              <span class="checkKey"></span>
              <span>】的结果</span></div>
          </div>


        </li>
          </ul>
    <div class="clear"></div>
  </div>
</div>
<script>
    var isLogin = '0';
    var userId = '';
    var imgpath = 'https://s2.51cto.com/';
    var BLOG_URL = 'https://blog.51cto.com/';
    var YII_ENV = 'prod';
    var router = 'blogger/index';
    var STATIC_IMG = 'https://static2.51cto.com/edu/blog/images/'
    localStorage.removeItem('userDraft')
    $('.want-write').click(function(){
        localStorage.removeItem('userDraft')
    })

</script>
<div class="Content-box">
    <link rel="stylesheet" href="https://static2.51cto.com/edu/blog/mobile/css/lib/swiper.css">
<script src="https://static2.51cto.com/edu/blog/mobile/js/lib/swiper.js?v1" charset="utf-8"></script>
<script>

var is_reload = true;
$(".follow-top").click(function() {
    is_reload = false;
})
function FollowBtnSucc(e){//1:未关注,2:已关注,3:互相关注
    if(e==2||e==3){
        boxProxy()
    }else{
        if(is_reload) {
            window.location.reload();
        }
    }
    is_reload = true;
}
</script>
<div class="bloger-content-new">
    <div class="banner">
        <div class="Page">
                            <h1 class="name">康建华</h1>
                        <nav class="clearfix">
                <ul class="clearfix">
                   <li  ><a href="https://blog.51cto.com/michaelkang/release">动态</a></li>
                   <li class="cur" ><a href="https://blog.51cto.com/michaelkang">博客</a></li>
                   <li ><a href="https://blog.51cto.com/michaelkang/classify">分类</a></li>
                   <li ><a href="https://blog.51cto.com/michaelkang/following">订阅/关注</a></li>
                </ul>
                <div class="search">
                    <form class="fr form-search" method='get' action="https://blog.51cto.com/search/user" target="_blank">
                        <input type="hidden" name="uid" value="1553154">
                        <input type="text"  name="q" placeholder="搜TA的内容"  maxlength="38" id="blogerSearchInput" autocomplete="off">
                        <button class="iconblog blogsou" id="blogerSearchBtn"></button>
                    </form>
                </div>
            </nav>
        </div>
    </div>
    <aside class="action-aside">
        <ul>
            <li>
                <strong class="sign" id="sign">
                    <a href="javascript:;">
                        <i class="iconblog blogqiandao"></i>
                                                <b class="dot"></b>
                                            </a>
                    <span>签到领勋章</span>
                </strong>
            </li>
            <li class="share">
                <strong class="">
                    <a href="javascript:;"><i class="iconblog blogfen"></i></a>
                    <span>分享</span>
                </strong>
            </li>
            <li class="scrollTop">
                <strong class="ScrollWindowTop">
                    <a href="javascript:;"><i class="iconblog blogzhi"></i></a>
                    <span>返回顶部</span>
                </strong>
            </li>
        </ul>
    </aside>
    <div class="clearfix Page">
       <aside class="bloger-content-left">
            <section class="common-section common-spacing mb24 user-intr">
                <div class="pic"><a href="https://blog.51cto.com/michaelkang"><img class="is-vip-img is-vip-img-5" data-uid="1553154" src="https://ucenter.51cto.com/images/noavatar_middle.gif" alt="无锋剑客"></a></div>
                <div class="clearfix username">
                    <h3 class="blog-user" title="无锋剑客" style="max-width: 262px;">无锋剑客</h3>
                    <div class="icon">
                        <ul class="clearfix detail-list">
                                                                                                                                                                    </ul>
					</div>
                </div>
                <div  class="identify-list">
                    <script id="identifyScript" type="text/html">
                        {{each data value index}}
                        <div class="item item{{value.type}}">
                            <span title="{{value.title}}">
                                {{if value.type==1}}
                                <i title="已通过员工认证"></i>
                                {{else if value.type==2}}
                                <i title="已通过学生认证"></i>
                                {{else if value.type==3}}
                                <i title="已通过教师认证"></i>
                                {{else if value.type==4}}
                                <i title="已通过企业认证"></i>
                                {{/if}}
                                {{value.title}}
                            </span>
                        </div>
                        {{/each}}
                    </script>
                </div>
                                                            <div class="dec"> 静静地努力，静静的收获，请勿喧哗！</div>
                                    

                <ul class="clearfix numsbox">
                    <li class="nums">
                        <strong>500.2万</strong>
                        <span>人气</span>
                    </li>
                    <li class="line"></li>
                    <li class="nums">
                        <a href="https://blog.51cto.com/michaelkang/original">
                        <strong>411</strong>
                        <span>原创</span>
                        </a>
                    </li>
                    <li class="nums">
                        <a href="https://blog.51cto.com/michaelkang/followers">
                        <strong>49</strong>
                        <span>粉丝</span>
                        </a>
                    </li>
                    <li class="line"></li>
                    <li class="nums">
                        <strong>233.7万</strong>
                        <span>阅读数</span>
                    </li>
                </ul>
                <div id="medalListBox" class="medal-list">
                    <script id="medalList" type="text/html">
                        {{each list}}
                            <div title="{{$value.name}}" class="item" id="medalItem">
                                <img src="{{$value.img_light}}">
                            </div>
                        {{/each}}
                    </script>
                </div>
                                    <div class="clearfix operating">
                        <button class="sx" data="https://home.51cto.com/space?uid=1553154" id="ToSx"><a href="javascript:;" rel="nofollow"><i class="iconblog blogsixin"></i>私信</a></button>

                                                    <a id="checkFollow_t_1553154" class="follow-1 follow-top checkFollow on" href="javascript:;">关注</a>
                                                <script>
                            FollowBtn = new Follow($('#checkFollow_t_1553154'),'1553154','1',['on','in','mutual','off'])
                            FollowBtn.success=FollowBtnSucc
                        </script>

                    </div>
                            </section>
            <section class="common-section common-spacing mb24 joinbox">
                <div class="joins">于 <span>2010-05-04</span> 加入 51CTO<span class="time">12.3年</span></div>
            </section>
                                                <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="感兴趣的领域">感兴趣的领域</h2>                </div>
                <div class="interestbox">
                                    <span>#集群</span>
                                    <span>#redis</span>
                                    <span>#云平台</span>
                                    <span>#自动化运维</span>
                                    <span>#Web服务器</span>
                                    <span>#MongoDB</span>
                                    <span>#Docker</span>
                                </div>
            </section>
                                    <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="热门文章">热门文章</h2>
                </div>
                <ul class="common-list common-list-dot">
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/5501454" target="_blank" title="spark-master 高可用测试">spark-master 高可用测试</a>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/5501446" target="_blank" title="linux系统使用arp-scan检查是否存在IP地址冲突">linux系统使用arp-scan检查是否存在IP地址冲突</a>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/5501457" target="_blank" title="Kubernetes1.15部署Dashboard">Kubernetes1.15部署Dashboard</a>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/5501447" target="_blank" title="linux系统内存转换成硬盘使用">linux系统内存转换成硬盘使用</a>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/5501455" target="_blank" title="Cassandra集群管理-节点异常重启">Cassandra集群管理-节点异常重启</a>
                        </li>
                                    </ul>
            </section>
                        <!-- 近期文章 -->
                        <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="近期文章">近期文章</h2>
                </div>
                <ul class="common-list">
                                        <li>
                        <a href="https://blog.51cto.com/michaelkang/5501457" target="_blank" title="Kubernetes1.15部署Dashboard">Kubernetes1.15部署Dashboard</a>
                    </li>
                                        <li>
                        <a href="https://blog.51cto.com/michaelkang/5501456" target="_blank" title="Cassandra 集群核心配置和概梳理">Cassandra 集群核心配置和概梳理</a>
                    </li>
                                        <li>
                        <a href="https://blog.51cto.com/michaelkang/5501455" target="_blank" title="Cassandra集群管理-节点异常重启">Cassandra集群管理-节点异常重启</a>
                    </li>
                                        <li>
                        <a href="https://blog.51cto.com/michaelkang/5501454" target="_blank" title="spark-master 高可用测试">spark-master 高可用测试</a>
                    </li>
                                        <li>
                        <a href="https://blog.51cto.com/michaelkang/5501453" target="_blank" title="kubernetes Ingress 之 Traefik 各种姿势">kubernetes Ingress 之 Traefik 各种姿势</a>
                    </li>
                                    </ul>
                <div class="common-list-lines"></div>
                                <div class="nowYear">
                    <div class="years">
                        2022年                    </div>
                    <div class="clearfix months">
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2022/month7" target="_blank">
                                <span>07月</span>
                                <strong>12篇</strong>
                            </a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2022/month1" target="_blank">
                                <span>01月</span>
                                <strong>1篇</strong>
                            </a>
                                            </div>
                </div>
                                                <div class="otherYear">
                    <div class="clearfix years">
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2021">2021年   2篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2020">2020年   13篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2019">2019年   110篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2018">2018年   63篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2017">2017年   30篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2016">2016年   35篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2015">2015年   20篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2014">2014年   24篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2013">2013年   82篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2012">2012年   61篇</a>
                                                    <a href="https://blog.51cto.com/michaelkang/article/year2011">2011年   17篇</a>
                                            </div>
                </div>
                            </section>
                                    <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="热门好文">热评好文</h2>
                </div>
                <ul class="common-list common-list-dot">
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2389520" target="_blank" title="kubernetes node 节点启动报错: No valid private key">kubernetes node 节点启动报错: No valid private key</a>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2387223" target="_blank" title="Gitlab-runner 构建失败问题排查">Gitlab-runner 构建失败问题排查</a>
                        </li>
                                    </ul>
            </section>
                                    <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="近期评论">近期评论</h2>
                </div>
                <ul class="common-list common-list-dot">
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2533103" target="_blank" title="分布式调度系统-DolphinScheduler">分布式调度系统-DolphinScheduler</a>
                            <p class="dec">新一代分布式大数据工作流任务调度系统DolphinScheduler源码分析
网盘地址：https://pan.baidu.com/s/1qT32V7cIggmBBifjC9oZHg 提取码: gafa
备用地址（腾讯微云）：https://share.weiyun.com/e4Ij0xF8 密码：n7jyha</p>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2431889" target="_blank" title="生产环境kubernetes集群安装部署-1.15.3">生产环境kubernetes集群安装部署-1.15.3</a>
                            <p class="dec">您好，https://gitlab.com/PtmindDev/devops/kub-deploy/tree/cn-k8s-prod上的项目找不到了，能否提供下ansible脚本。非常感谢</p>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2429929" target="_blank" title="kubernetes Ingress 之 Traefik 各种姿势">kubernetes Ingress 之 Traefik 各种姿势</a>
                            <p class="dec">老师 问下使用多个traefik controller 。traefik controller 中如何配置ingress-class ？</p>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2389520" target="_blank" title="kubernetes node 节点启动报错: No valid private key">kubernetes node 节点启动报错: No valid private key</a>
                            <p class="dec">还是不行啊，依然看不到csr请求</p>
                        </li>
                                            <li>
                            <a  class="title" href="https://blog.51cto.com/michaelkang/2387223" target="_blank" title="Gitlab-runner 构建失败问题排查">Gitlab-runner 构建失败问题排查</a>
                            <p class="dec">报这样的错误，有遇到的吗？

Running with gitlab-runner 14.10.1 (f761588f)
  on cicd 8hAz17qH
Preparing the &quot;shell&quot; executor 00:00
Using Shell executor...
Preparing environment 00:00
bash: bash: command not found
ERROR: Job failed: prepare environment: exit status 127. Check https://docs.gitlab.com/runner/shells/index.html#shell-profile-loading for more information</p>
                        </li>
                                    </ul>
            </section>
                                    <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="七日热门">七日热门</h2>  <a href="https://blog.51cto.com/nav"  target="_blank">全部文章</a>
                </div>


                <div class="Box_content22">
                                                          <div class="Box-item-content">
                                  <div class="Box_content22_title">
                                     <div class='cir'></div>
                                     <a href="https://blog.51cto.com/u_15127637/4377554" target="_blank">elasticsearch 集群管理（集群规划、集群搭建、集群管理）</a>
                                  </div>
                                                                    <div class=" swiper-container11">
                                  <div class="tag-box">

                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/search/result?q=%E6%95%B0%E6%8D%AE" class="fl"  target="_blank">数据</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/elasticsearch.html" class="fl"  target="_blank">elasticsearch</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/html.html" class="fl"  target="_blank">html</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/search/result?q=%E6%90%9C%E7%B4%A2" class="fl"  target="_blank">搜索</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/search/result?q=%E9%AB%98%E5%8F%AF%E7%94%A8" class="fl"  target="_blank">高可用</a>
                                            </div>
                                                                      </div>
                              </div>
                              
                              </div>
                                                          <div class="Box-item-content">
                                  <div class="Box_content22_title">
                                     <div class='cir'></div>
                                     <a href="https://blog.51cto.com/u_15061944/4054192" target="_blank">ES 集群管理（集群规划、集群搭建、集群管理）</a>
                                  </div>
                                                                    <div class=" swiper-container11">
                                  <div class="tag-box">

                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl"  target="_blank">数据</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/elasticsearch.html" class="fl"  target="_blank">elasticsearch</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/sousuo.html" class="fl"  target="_blank">搜索</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/html.html" class="fl"  target="_blank">html</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/fangwenxianzhi.html" class="fl"  target="_blank">访问限制</a>
                                            </div>
                                                                      </div>
                              </div>
                              
                              </div>
                                                          <div class="Box-item-content">
                                  <div class="Box_content22_title">
                                     <div class='cir'></div>
                                     <a href="https://blog.51cto.com/u_12890843/5349370" target="_blank">redis 集群 kafka集群 zk集群</a>
                                  </div>
                                                                    <div class=" swiper-container11">
                                  <div class="tag-box">

                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/kafka.html" class="fl"  target="_blank">kafka</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/zookeeper.html" class="fl"  target="_blank">zookeeper</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/html.html" class="fl"  target="_blank">html</a>
                                            </div>
                                                                      </div>
                              </div>
                              
                              </div>
                                                          <div class="Box-item-content">
                                  <div class="Box_content22_title">
                                     <div class='cir'></div>
                                     <a href="https://blog.51cto.com/u_15076233/4121459" target="_blank">Zookeeper 集群 + Kafka 集群</a>
                                  </div>
                                                                    <div class=" swiper-container11">
                                  <div class="tag-box">

                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/zookeeper.html" class="fl"  target="_blank">zookeeper</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/fuwuqi.html" class="fl"  target="_blank">服务器</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl"  target="_blank">数据</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/apache.html" class="fl"  target="_blank">apache</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/kehuduan.html" class="fl"  target="_blank">客户端</a>
                                            </div>
                                                                      </div>
                              </div>
                              
                              </div>
                                                          <div class="Box-item-content">
                                  <div class="Box_content22_title">
                                     <div class='cir'></div>
                                     <a href="https://blog.51cto.com/u_15064643/4170207" target="_blank">Zookeeper集群+kafka集群</a>
                                  </div>
                                                                    <div class=" swiper-container11">
                                  <div class="tag-box">

                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/zookeeper.html" class="fl"  target="_blank">zookeeper</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/kafka.html" class="fl"  target="_blank">kafka</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/fuwuqi.html" class="fl"  target="_blank">服务器</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl"  target="_blank">数据</a>
                                            </div>
                                                                                    <div class="tag-item">
                                                <a href="https://blog.51cto.com/topic/xiaoxiduilie.html" class="fl"  target="_blank">消息队列</a>
                                            </div>
                                                                      </div>
                              </div>
                              
                              </div>
                                                  </div>
            </section>
                        <!-- 分类 -->

            <section class="common-section common-spacing mb24 classification_000" id="Classification_648">
                <div class="clearfix common-sub-title">
                    <h2 title="Ta的分类">Ta的分类</h2>
                </div>
                <ul class="common-list common-list-dot" id="classification_001">

                </ul>
                <div class="Classification_648_add" id="Classification_648_add" onclick="addClassification(1)">加载更多</div>
            </section>
                        <section class="common-section common-spacing mb24">
                <div class="clearfix common-sub-title">
                    <h2 title="近期来访">近期来访</h2>
                </div>
                <ul class="clearfix guestbox">
                                    <li>
                        <div class="pic">
                            <a href="https://blog.51cto.com/u_15398665">
                            <img class="is-vip-img is-vip-img-5" data-uid="15388665" src="https://ucenter.51cto.com/images/noavatar_middle.gif">
                            </a>
                        </div>
                        <div class="name"><a href="https://blog.51cto.com/u_15398665" title="">51CTO博客运营-可可</a></div>
                    </li>
                                        <li>
                        <div class="pic">
                            <a href="https://blog.51cto.com/u_15590126">
                            <img class="is-vip-img is-vip-img-5" data-uid="15580126" src="https://ucenter.51cto.com/images/noavatar_middle.gif">
                            </a>
                        </div>
                        <div class="name"><a href="https://blog.51cto.com/u_15590126" title="">wx624ea057c70c3</a></div>
                    </li>
                                        <li>
                        <div class="pic">
                            <a href="https://blog.51cto.com/u_15327680">
                            <img class="is-vip-img is-vip-img-5" data-uid="15317680" src="https://ucenter.51cto.com/images/noavatar_middle.gif">
                            </a>
                        </div>
                        <div class="name"><a href="https://blog.51cto.com/u_15327680" title="">ERROR.</a></div>
                    </li>
                                        <li>
                        <div class="pic">
                            <a href="https://blog.51cto.com/u_14517982">
                            <img class="is-vip-img is-vip-img-5" data-uid="14507982" src="https://ucenter.51cto.com/images/noavatar_middle.gif">
                            </a>
                        </div>
                        <div class="name"><a href="https://blog.51cto.com/u_14517982" title="">flyele</a></div>
                    </li>
                                        <li>
                        <div class="pic">
                            <a href="https://blog.51cto.com/u_15545633">
                            <img class="is-vip-img is-vip-img-5" data-uid="15535633" src="https://ucenter.51cto.com/images/noavatar_middle.gif">
                            </a>
                        </div>
                        <div class="name"><a href="https://blog.51cto.com/u_15545633" title="">wx622ba8eeae50b</a></div>
                    </li>
                                    </ul>
            </section>
                   </aside>
       <div class="bloger-content-right">
                          <section class="common-section common-spacing" id="common-section-one">




    <div class="conditions">
        <ul class="clearfix">
            <li class="sortajax"><a class="first" href="javascript:;" class="first" sort="published">按发布时间</a></li>
            <li class="sortajax"><a class="first" href="javascript:;" class="first" sort="views">按阅读量</a></li>
                        <li class="time-line conditions-right">
                <a href="" class="first">时间轴<i class="iconblog blogzhankai"></i></a>
                <div class="hideItem">
                    <div class="inner">
                                                    <a href="/michaelkang" class="                                            total"
                                            ><span>全部</span><strong>470篇</strong>
                    </a>
                    <div class="timelist">                                                                            <a href="/michaelkang/article/year2022" class="                                            year clearfix"
                                            ><span>2022年</span><strong>13篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2022/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>12篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2022/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2021" class="                                            year clearfix"
                                            ><span>2021年</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2021/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020" class="                                            year clearfix"
                                            ><span>2020年</span><strong>13篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2020/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019" class="                                            year clearfix"
                                            ><span>2019年</span><strong>110篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month12" class="                                            month clearfix"
                                            ><span>12月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>26篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>17篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month6" class="                                            month clearfix"
                                            ><span>06月</span><strong>16篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>13篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>19篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2019/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018" class="                                            year clearfix"
                                            ><span>2018年</span><strong>63篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month12" class="                                            month clearfix"
                                            ><span>12月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>12篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>21篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>14篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2018/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>7篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017" class="                                            year clearfix"
                                            ><span>2017年</span><strong>30篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month12" class="                                            month clearfix"
                                            ><span>12月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>7篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>10篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2017/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016" class="                                            year clearfix"
                                            ><span>2016年</span><strong>35篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month6" class="                                            month clearfix"
                                            ><span>06月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>22篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2016/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015" class="                                            year clearfix"
                                            ><span>2015年</span><strong>20篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month12" class="                                            month clearfix"
                                            ><span>12月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2015/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014" class="                                            year clearfix"
                                            ><span>2014年</span><strong>24篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>6篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>6篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2014/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013" class="                                            year clearfix"
                                            ><span>2013年</span><strong>82篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>4篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>6篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>11篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month6" class="                                            month clearfix"
                                            ><span>06月</span><strong>9篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>19篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>8篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>9篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2013/month1" class="                                            month clearfix"
                                            ><span>01月</span><strong>8篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012" class="                                            year clearfix"
                                            ><span>2012年</span><strong>61篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month12" class="                                            month clearfix"
                                            ><span>12月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month11" class="                                            month clearfix"
                                            ><span>11月</span><strong>15篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>9篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>5篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month6" class="                                            month clearfix"
                                            ><span>06月</span><strong>8篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>3篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2012/month2" class="                                            month clearfix"
                                            ><span>02月</span><strong>10篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011" class="                                            year clearfix"
                                            ><span>2011年</span><strong>17篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month10" class="                                            month clearfix"
                                            ><span>10月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month9" class="                                            month clearfix"
                                            ><span>09月</span><strong>10篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month8" class="                                            month clearfix"
                                            ><span>08月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month7" class="                                            month clearfix"
                                            ><span>07月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month5" class="                                            month clearfix"
                                            ><span>05月</span><strong>1篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month4" class="                                            month clearfix"
                                            ><span>04月</span><strong>2篇</strong>
                    </a>
                                                                                                <a href="/michaelkang/article/year2011/month3" class="                                            month clearfix"
                                            ><span>03月</span><strong>1篇</strong>
                    </a>
                                                             </div>                                    </div>
                </div>
            </li>
                                         <li class="conditions-right"><a  class="first clearfix"  href="/michaelkang/push"><i class="iconblog blogweixuanzhongbeifen"></i>推荐</a></li>
                         <li class="article-type conditions-right">
                                                                                                                                                                                                                                    <a href="" class="first">全部<i class="iconblog blogzhankai"></i></a>
                                <div class="hideItem">
                    <div class="inner">
                                                    <a href="/michaelkang" class="cur">全部</a>
                                                                            <a href="/michaelkang/original" >原创</a>
                                                    <a href="/michaelkang/reproduce" >转载</a>
                                                    <a href="/michaelkang/translate" >翻译</a>
                                            </div>
                </div>
            </li>
        </ul>
    </div>
            
    <div class="common-article-listbox" id="common-article-listbox-1">
                    <div class="common-article-list">
            <div class="clearfix graphic">
                   
                    <a class="pic" href="https://blog.51cto.com/michaelkang/5501457" target="_blank">
                        <img src="https://s2.51cto.com/images/blog/202207/12153909_62cd251d3b5e71750.png?x-oss-process=image/resize,m_fixed,w_116,h_70/format,webp/ignore-error,1" alt="Kubernetes1.15部署Dashboard">
                                            </a>   
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501457" target="_blank">Kubernetes1.15部署Dashboard</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501457" target="_blank">=== master节点上进行如下操作 ===部署方法1-原生文件部署：kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v1.10.1/src/deploy/recommended/kubernetes-dashboard.yaml默认使用端口：8001默认镜像下载地址：google部署方法2...</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/github.html" class="fl" target="_blank">github</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/sed.html" class="fl" target="_blank">sed</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/5e.html" class="fl" target="_blank">5e</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>56</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501456" target="_blank">Cassandra 集群核心配置和概梳理</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501456" target="_blank">Cassandra是一款分布式的结构化数据存储方案(NoSql数据库)，存储结构比Key-Value数据库（像Redis）更丰富，但是比Document数</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl" target="_blank">数据</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/huancun.html" class="fl" target="_blank">缓存</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/fuwuqi.html" class="fl" target="_blank">服务器</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>41</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501455" target="_blank">Cassandra集群管理-节点异常重启</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501455" target="_blank">Cassandra集群管理-节点异常重启登陆一台集群节点，直接重启服务器(172.20.101.166)，设置了 cassandra </a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/java.html" class="fl" target="_blank">java</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/chongqi.html" class="fl" target="_blank">重启</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/apache.html" class="fl" target="_blank">apache</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>52</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501454" target="_blank">spark-master 高可用测试</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501454" target="_blank">spark-master 高可用测试：集群介绍[spark-m]172.20.101.157 sparkname=master01 172.20.101.164 sparkname=master02172.20.101.165 sparkname=master03 [spark-s]172.20.101.160 sparkname=slave01 172.20.101.166 s...</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/spark.html" class="fl" target="_blank">spark</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/hadoop.html" class="fl" target="_blank">hadoop</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/zookeeper.html" class="fl" target="_blank">zookeeper</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>66</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501453" target="_blank">kubernetes Ingress 之 Traefik 各种姿势</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501453" target="_blank">关于traefik参考之前写的一篇文档：​​https://blog.51cto.com/michaelkang/1918192​​版本介绍traefik：v1.7k8s：v1.15.1IngressIngress是自kubernetes1.1版本后引入的资源类型。必须要部署Ingress controller才能创建Ingress资源，Ingress controller是以一种插件的形式提供。</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/java.html" class="fl" target="_blank">java</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/kubernetes.html" class="fl" target="_blank">kubernetes</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/docker.html" class="fl" target="_blank">docker</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/python.html" class="fl" target="_blank">python</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/linux.html" class="fl" target="_blank">linux</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>42</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501452" target="_blank">K8s之traefik（ingess）发布服务-实战</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501452" target="_blank">K8s之traefik（ingess）发布服务实战上篇描述了基于k8s集群安装部署traefik作为ingress服务，简单演示了一下发布服务</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/f5.html" class="fl" target="_blank">f5</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/html.html" class="fl" target="_blank">html</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/h5.html" class="fl" target="_blank">h5</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>33</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501450" target="_blank">删除Rancher的空间cattle-system,状态一直是Terminating</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501450" target="_blank">故障现象使用Rancher2.0代理了Kubernetes的管理web页面。因未知原因，Rancher服务无法启用，删除Rancher依赖的na</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/webyemian.html" class="fl" target="_blank">web页面</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>41</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501449" target="_blank">linux sar 命令详解</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501449" target="_blank">sar（System Activity Reporter系统活动情况报告）是目前 Linux 上最为全面的系统性能分析工具之一，可以从多方面对系统的活动进行报告，包括：文件的读写情况、系统调用的使用情况、磁盘I/O、CPU效率、内存使用状况、进程活动及IPC有关的活动等。本文主要以CentOS 6.3 x64系统为例，介绍sar命令。sar命令常用格式sar [options] [-</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/pingmuxianshi.html" class="fl" target="_blank">屏幕显示</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/wulishebei.html" class="fl" target="_blank">物理设备</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/sed.html" class="fl" target="_blank">sed</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>20</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501448" target="_blank">linux下测试磁盘的读写IO速度</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501448" target="_blank">有时候我们在做维护的时候，总会遇到类似于IO特别高，但不能判定是IO瓶颈还是软件参数设置不当导致热盘的问题.这时候</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/ide.html" class="fl" target="_blank">ide</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/linux.html" class="fl" target="_blank">linux</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/huancun.html" class="fl" target="_blank">缓存</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>30</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501447" target="_blank">linux系统内存转换成硬盘使用</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501447" target="_blank">解决问题点：1：站点数据提速，数据放入内存空间，速度指数级提升；2：数据库缓存；3：临时数据处理；4：等等。。。#查</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/5g.html" class="fl" target="_blank">5g</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/neicunkongjian.html" class="fl" target="_blank">内存空间</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/yace.html" class="fl" target="_blank">压测</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>55</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5501446" target="_blank">linux系统使用arp-scan检查是否存在IP地址冲突</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5501446" target="_blank">                   linux系统使用arp-scan检查是否存在IP地址冲突	如果前期没有做好IP地址规划，即使有IP地址统一不小心也会犯</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/ipdizhi.html" class="fl" target="_blank">ip地址</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/fuwuqi.html" class="fl" target="_blank">服务器</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/macdizhi.html" class="fl" target="_blank">mac地址</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>59</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">14 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5479297" target="_blank">linux sysctl -p 报error:</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5479297" target="_blank">修改 linux 内核文件 sysctl -P 报错error: "net.bridge.bridge-nf-call-ip6tables" is an unknown key error: "net.bridge.bridge-nf-call-iptables" is an unknown key error: "ne...</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/linux.html" class="fl" target="_blank">linux</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/yunwei.html" class="fl" target="_blank">运维</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/fuwuqi.html" class="fl" target="_blank">服务器</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/jiejuefangfa.html" class="fl" target="_blank">解决方法</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>22</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">22 天前</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/4907256" target="_blank">Configmap&amp;Secret 结合Reloader实现服务热更新</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/4907256" target="_blank">业务环境进行服务构建或者部署时经常遇到一个问题,就是不同的环境要配置不同的资源信息.有些资源信息还比较敏感,在构建过程总导出传递,容易产生信息泄露,存在较大的安全隐患.在容器化时代结合 K8S 集群运行服务,通常会依赖 Configmap 或者 Secret 来解决此类问题.</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/search/result?q=%E5%BA%94%E7%94%A8%E7%A8%8B%E5%BA%8F" class="fl" target="_blank">应用程序</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/github.html" class="fl" target="_blank">github</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/config.html" class="fl" target="_blank">config</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/map.html" class="fl" target="_blank">map</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/secret.html" class="fl" target="_blank">secret</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>287</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2022-01-10</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2607115" target="_blank">Curl 请求输出网络耗时</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2607115" target="_blank">目的curl请求页面时打印请求过程中的耗时，方便识别网络过程中存在问题。生成打印字段配置文件：cat&gt;./curl-format.txt&lt;&lt;-EOFtime_namelookup:%{time_namelookup}\ntime_connect:%{time_connect}\ntime_appconnect:%{time_appconnect}\ntime_redirect:%</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/curl.html" class="fl" target="_blank">Curl </a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/qingqiushuchu.html" class="fl" target="_blank">请求输出</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/wangluo.html" class="fl" target="_blank">网络</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/haoshi2.html" class="fl" target="_blank">耗时</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag reprint fl">转载</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>3548</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>1</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2021-01-26</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2580660" target="_blank">Serverless（无服务器）架构知识梳理</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2580660" target="_blank">前题：大多数公司在开发应用程序并将其部署在服务器上的时候，无论是选择公有云还是私有的数据中心，都需要提前了解究竟需要多少台服务器、多大容量的存储和数据库的功能等。并需要部署运行应用程序和依赖的软件到基础设施之上。如果我们不想在这些细节上花费精力，是否有一种简单的架构模型能够满足我们这种想法？这个答案已经存在，这就是今天软件架构世界中新鲜但是很热门的一个话题——Serverless（无服务器）架构。</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/serverless.html" class="fl" target="_blank">Serverless</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/wufuwuqi.html" class="fl" target="_blank">无服务器</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/jiagou.html" class="fl" target="_blank">架构</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/zhishi.html" class="fl" target="_blank">知识</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag reprint fl">转载</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>895</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2021-01-02</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2553883" target="_blank">企业数据驱动最难攻克的高地在哪里？</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2553883" target="_blank">前提很多企业喊着要数据驱动，网络上是各种技术、解决方案的推广，面板展示高端炫酷，感觉好像是公司有数了，大屏展示了！就算数据驱动了？就能数据驱动了？概念我们先简单回答一下数据驱动的概念：数据驱动是指将数据作为生产资料，通过科学的方法，在业务实践中不断作出正向的反馈，促进业务优化提高。不知道大家发现了吗？这个概念描述跟学术，里面没有任何人的字眼提及。这个挺坑的，从个人推进公司数据驱动相关事情的感受来讲</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/qiyeshuju.html" class="fl" target="_blank">企业数据</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/qudong.html" class="fl" target="_blank">驱动</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>477</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-11-24</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2547496" target="_blank">笔记-如何在实际工作中使用数据</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2547496" target="_blank">原文转载地址：头条号IT思维前提：数据啊数据，到处都在喊数据，确实我们每个人的身边都围绕着各种数据，数据时代，我们工作周边也都是数据，用数据解决实际问题的能力，已经成为大数据时代人人必备的硬实力之一。我们从哪里开始迈出第一步？出发前准备为了在有限的时间里取得一定的成果，建议大家从一开始就对整体计划和“地图”做到心中有数。目的很重要抱着“先从容易收集的数据开始统计”的想法进行分析，这本身就是错的。正</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shijigongzuo.html" class="fl" target="_blank">实际工作</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shiyongshuju.html" class="fl" target="_blank">使用数据</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag reprint fl">转载</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>708</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-11-07</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2547485" target="_blank">数据质量管理</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2547485" target="_blank">转载地址：IT思维前提：数据时代，数据产生的价值越来越大，基于数据的相关技术，应用形式也快速发展，当前各大厂商、用户都在探索与数据相关的开发技术、应用场景和商业模式，最终目的就是挖掘数据价值，推动业务发展。而只有高质量的数据才能够真正意义上实现数据价值的最大化，没有数据治理，没有数据质量的保证，再多的业务和技术的投入，都可能是徒劳的。背景公司经过多年信息化系统建设和应用，积累了大量的数据信息,这些</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl" target="_blank">数据</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/zhiliang.html" class="fl" target="_blank">质量</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/guanli.html" class="fl" target="_blank">管理</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/guocheng.html" class="fl" target="_blank">过程</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>812</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-11-07</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2533113" target="_blank">BI的过去和未来</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2533113" target="_blank">原文转载地址：头条号IT思维什么是BIBusinessIntelligence，简称：BI，又称商业智慧或商务智能，指用现代数据仓库技术、线上分析处理技术、数据挖掘和数据展现技术进行数据分析以实现商业价值。作用商业智能作为一个平台工具，处理企业中现有数据，并将其转换成知识、分析和结论，辅助业务或者决策者做出正确且明智的决定，帮助企业更好地利用数据提高决策质量的技术。不仅为企业提供信息获取能力，而且</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/bi.html" class="fl" target="_blank">BI</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/guoqu.html" class="fl" target="_blank">过去</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/weilai.html" class="fl" target="_blank">未来</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>597</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-09-14</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2533111" target="_blank">开源BI平台软件特性对比</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2533111" target="_blank">数据时代来临，随着更多的社会资源进行网络化和数据化改造，数据所能承载的价值也必将不断提到提高。与此同时数据正在成为企业重要的生产材料之一，企业可以通过数据来完成产品（服务）的设计、创新，同时基于数据也能够全面赋能企业的运营管理。</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/kaiyuan.html" class="fl" target="_blank">开源</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/bi.html" class="fl" target="_blank">BI</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/ruanjiantexing.html" class="fl" target="_blank">软件特性</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/duibi.html" class="fl" target="_blank">对比</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>1</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>3115</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-09-14</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2533103" target="_blank">分布式调度系统-DolphinScheduler</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2533103" target="_blank">原文转载地址：头条号IT思维前提数据平台（BP）建设过程中，会涉及大量的数据采集、处理、计算等方面的工作，而且随着需求的增加要承担的任务越来越多。迫切需要一个简单易用、支持可视化管理的调度系统，考虑到要将现有的定时任务从crontab快速迁移到新调度系统，且要易于部署管理，方便扩展，支持HA等要求。调研了多款调度系统如airflow、azkaban、gocron、DolphinScheduler等</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/fenbushidiaoduxitong.html" class="fl" target="_blank">分布式调度系统</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/dolphinsched.html" class="fl" target="_blank">DolphinSched</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shuju.html" class="fl" target="_blank">数据</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/pingtai.html" class="fl" target="_blank">平台</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>4953</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>1</b>
                    </span>
                                        <span class="actions fr">2020-09-14</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2530390" target="_blank">ES创建index报错cluster currently has 4/2 maximum shard</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2530390" target="_blank">原文链接IT思维前提调试业务服务期间，服务日志需要写入es集群，发现数据写入报错。报错内容如下ElasticsearchDeprecationWarning:Inafuturemajorversion,thisrequestwillfailbecausethisactionwouldadd[10]totalshards,butthisclustercurrentlyhas[20242]/[2000</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/chuangjianindex.html" class="fl" target="_blank">创建index</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/baocuo.html" class="fl" target="_blank">报错</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/maximum.html" class="fl" target="_blank">maximum </a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/shards.html" class="fl" target="_blank">shards</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/open.html" class="fl" target="_blank">open</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>1601</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-09-08</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2494736" target="_blank">k8s集群拉取镜像报错:not exist or may require docker login</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2494736" target="_blank">前提新启动一个Rancher管理集群，将原有集群作为资源集群加入Rancher管理集群，提升集群稳定性和安全性。集群合并调整期间顺利完成，集群升级完成后，原Rancher集群升级业务服务时发现报错如下：ErrImagePull:rpcerror:code=Unknowndesc=Errorresponsefromdaemon:pullaccessdeniedforreg.itsiv.com/lin</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/kubernetes.html" class="fl" target="_blank">kubernetes</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/qujingxiangbaocuo.html" class="fl" target="_blank">取镜像报错</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/dockerlogin.html" class="fl" target="_blank">docker login</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/notexist.html" class="fl" target="_blank">not exist</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>3351</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-05-12</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2491951" target="_blank">Traefik2.2.0 安装部署详解</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2491951" target="_blank">转载地址原站地址请添加链接描述前提：Traefik2.X.0现已发布一段时间，版本更新不少新特性,尤其是TCP转发和http转发并存这个亮点，可以解决不少业务问题，节省很多核心网络端口，特裸机部署进行体验。核心概念Traefik类似边缘路由器，可以作为整个平台的入口，根据逻辑和规则，处理并路由每个传入的请求。这些规则确定哪些服务处理哪些请求；传统的反向代理需要一个配置文件，其中包含路由到你服务的所</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/traefik220.html" class="fl" target="_blank">Traefik2.2.0</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/anzhuangbushu.html" class="fl" target="_blank">安装部署</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/xiangjie.html" class="fl" target="_blank">详解</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>5007</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-04-30</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2491751" target="_blank">容器化时代ab压测工具新用法</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2491751" target="_blank">转载地址原文地址目标：通过apacheab工具进行性能简单压测，获取服务性能。ab特点：ab是针对HTTP服务进行性能压力测试的工具，它最初被设计用来测量Apache服务器的性能指标，主要用来测试Apache服务器每秒能够处理多少请求以及响应时间，但这个命令也可以用来测试通用的HTTP服务性能。运行方式：ab-k-n10000-c30http://domain.com常用参数：-cconcurre</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/abdockerrongqi.html" class="fl" target="_blank">ab、docker、容器</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>1279</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-04-30</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2483251" target="_blank">KUBERNETES服务健康检查配置最佳实践</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2483251" target="_blank">原文转载地址；https://www.itsiv.com/2020/03/30/kubernetes%e6%9c%8d%e5%8a%a1%e5%81%a5%e5%ba%b7%e6%a3%80%e6%9f%a5%e5%8a%9f%e8%83%bd%e6%a2%b3%e7%90%86/简介K8S服务健康从两个维度进行分别为：就绪状态检查(readiness)和存活状态检查(liveness)。存活探针</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/kubernetes.html" class="fl" target="_blank">KUBERNETES</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/fuwujiankangjiancha.html" class="fl" target="_blank">服务健康检查</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/readiness.html" class="fl" target="_blank">readiness</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/livenees.html" class="fl" target="_blank">livenees</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag reprint fl">转载</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>1976</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-03-30</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2469087" target="_blank">kubectl 创建服务报no matches version extensions/v1beta1</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2469087" target="_blank">故障现象：执行kubectlcreate-ffilebeat.yml报错如下：error:unabletorecognize"filebeat.yml":nomatchesforkind"DaemonSet"inversion"extensions/v1beta1"解决办法：将yml配置文件内的api接口修改为apps/v1，导致原因为之间使用的kubernetes版本是1.14.x版本，1.16</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/kubectl.html" class="fl" target="_blank">kubectl</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/chuangjianfuwu.html" class="fl" target="_blank">创建服务</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/matches.html" class="fl" target="_blank">matches</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/extensionsv1beta1.html" class="fl" target="_blank">extensions/v1beta1</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>3631</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-02-04</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2464508" target="_blank">traefik使用etcd存储配置--实例演示</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2464508" target="_blank">traefik使用etcd作为后端配置存储配置实例功能测试目的：1：Traefik作为web服务，使用etd库作为配置统一存储空间，实现traefik服务可以方便的增删节点，解耦traefik服务启动后服务配置的问题。2：Traefik使用http验证方式申请ssl证书，即每配置一个域名让traefik帮我们自动申请一个ssl证书.测试步骤如下：1：安装traefik1.7+2：安装etcd3：安</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/traefik.html" class="fl" target="_blank">traefik</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/etcd.html" class="fl" target="_blank">etcd</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/ssl.html" class="fl" target="_blank">ssl</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/etcdkeeper.html" class="fl" target="_blank">etcdkeeper </a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/acme.html" class="fl" target="_blank">acme</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>1573</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2020-01-05</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/2460162" target="_blank">Gitlab https拉取代码缓存用户密码配置小记</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/2460162" target="_blank">起因业务服务器安全加固不再允许使用个人私有key配置再服务器，为了配置调试方便使用https方式拉取代码，但是发现每次Gitpull、push都要输入用户和密码，很不方便，特整理此配置。永久记住密码会在用户家目录的.gitconfig文件中生成下面的配置。如果没有--global，则在当前项目下的.git/config文件中添加。gitconfig--globalcredential.helper</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/gitlab.html" class="fl" target="_blank">gitlab </a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/https.html" class="fl" target="_blank">https</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/laqudai.html" class="fl" target="_blank">拉取代</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/mahuancunyonghu.html" class="fl" target="_blank">码缓存用户</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>3829</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2019-12-19</span>
                                    </div>

            </div>
                    <div class="common-article-list">
            <div class="clearfix graphic">
                                <h3 class="title"><a href="https://blog.51cto.com/michaelkang/5467875" target="_blank">Gitlab https拉取代码缓存用户密码配置小记</a></h3>
                <p class="dec"><a href="https://blog.51cto.com/michaelkang/5467875" target="_blank">起因业务服务器安全加固不再允许使用个人私有key配置再服务器，为了配置调试方便使用https方式拉取代码，但是发现每次Git pull 、push 都要输入用户和密码，很不方便，特整理此配置。永久记住密码会在用户家目录的.gitconfig文件中生成下面的配置。如果没有--global，则在当前项目下的.git/config文件中添加。git config --global credent...</a></p>
                                    <div class="tag-box">
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/git.html" class="fl" target="_blank">git</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/jizhumima.html" class="fl" target="_blank">记住密码</a>
                            </div>
                                                    <div class="tag-item">
                                <a href="https://blog.51cto.com/topic/zidingyi.html" class="fl" target="_blank">自定义</a>
                            </div>
                                            </div>
                              </div>
                <div class="clearfix messages">
                                                                <span class="tag original fl">原创</span>
                                                            <span class="nums fl " style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>0</b>
                    </span>
                                            <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>84</b>
                        </span>
                    
                    <span class="nums fl">
                        <i class="iconblog blogshoucang"></i>收藏<b>0</b>
                    </span>
                    <span class="nums fl">
                        <i class="iconblog blogpinglun1"></i>评论<b>0</b>
                    </span>
                                        <span class="actions fr">2019-12-19</span>
                                    </div>

            </div>
            </div>
<div class="common-article-listbox">
    <script id="articleListboxScript" type="text/html">
    {{each list value index}}
    <div class="common-article-list">
         <div class="clearfix graphic">
                    {{if value.img_urls && value.img_urls.length>0}}
                    <a href="{{value.url}}" class="pic" target="_blank">
                        <img src="{{value.img_urls[0]}}" alt="{{value.title}}">
                        {{if value.img_urls.length>1}}
                        <span>3图</span>
                        {{/if}}
                    </a>
                    {{/if}}
        <h3 class="title"><a href="{{value.url}}" target="_blank">{{value.title}}</a></h3>
        <p class="dec"><a href="{{value.url}}" target="_blank">{{value.abstract}}</a></p>        
        </div>
        <div class="clearfix messages">
            {{if value.top_time != '0'}}
            <span class="tag up fl">置顶</span>
            {{/if}}
            {{if value.blog_type == 1}}
            <span class="tag original fl">原创</span>
            {{else if value.blog_type == 2}}
                <span class="tag reprint fl">转载</span>
                {{else if value.blog_type == 3}}
                    <span class="tag translation fl">翻译</span>
                    {{/if}}
                    {{if value.level == 20}}
                    <span class="tag tuijian fl">推荐</span>
                    {{/if}}
                    <span class="nums fl {{value.is_praise}}" style="margin-left: 17px;">
                        <i class="iconblog blogdianzan" style="font-size:16px"></i>点赞<b>{{value.apraise_num}}</b>
                    </span>
                    {{if value.pv == '10000+'}}
                    <span class="nums fl">
                        <i class="iconblog blogyuedu1"></i>阅读<b>10000+</b>
                    </span>
                    {{else}}
                        <span class="nums fl">
                            <i class="iconblog blogyuedu1"></i>阅读<b>{{value.pv}}</b>
                        </span>
                        {{/if}}

                        <span class="nums fl">
                            <i class="iconblog blogshoucang"></i>收藏<b>{{value.favorite_num}}</b>
                        </span>
                        <span class="nums fl">
                            <i class="iconblog blogpinglun1"></i>评论<b>{{value.comments_num}}</b>
                        </span>
                        {{if value.flag}}
                            <a {{if value.img_urls && value.img_urls.length>0}}style="right:210px"{{/if}} href="{{value.subject.url}}" class="list-subjuct fr" target="_blank">
                                <i class="iconblog bloghuati fontsizeIcon"></i>
                                <span title="#{{value.subject.title}}#">#{{value.subject.title}}#</span>
                            </a>
                        {{/if}}
                        <span class="actions fr">{{value.add_time_str}}</span>
                        {{if value.delete_url != '' && value.is_check == 1}}
                            {{if value.top_time == '0'}} 
                            <span class="actions fr placeTop" data-id="{{value.blog_id}}" top_type="0">置顶</span>
                            {{else}}
                            <span class="actions fr placeTop" data-id="{{value.blog_id}}" top_type="1">取消置顶</span>
                            {{/if}}                       
                        {{/if}}

        </div>
    </div>
    {{/each}}
    {{if pagination !=''}}
    {{@pagination}}
    {{/if}}
    </script>
</div>        <ul class="pagination"><li class="first" style="display: none;"><span>首页</span></li>
<li class="prev" style="display: none;"><span></span></li>
<li class="active"><b>1</b></li>
<li><a href="https://blog.51cto.com/michaelkang/p_2" data-page="1">2</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_3" data-page="2">3</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_4" data-page="3">4</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_5" data-page="4">5</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_6" data-page="5">6</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_7" data-page="6">7</a></li>
<li><a href="https://blog.51cto.com/michaelkang/p_8" data-page="7">8</a></li>
<li class="next"><a href="https://blog.51cto.com/michaelkang/p_2" data-page="1"></a></li>
<li class="last"><a href="https://blog.51cto.com/michaelkang/p_16" data-page="15"></a></li>
<li class="last" style="display: none;"><span>共470条记录</span></li></ul>    </section>
                  </div>
   </div>
</div>
<script>
     var conditionparams = {"domain":"michaelkang"};
     var shareimgSrc =  'https://blog.51cto.com/qr/qr-url?url=https%3A%2F%2Fblog.51cto.com%2Fmichaelkang'

    window._bd_share_config={
    "common":{
      "bdText":"",
      "bdDesc":$("#abstract_bdshare").text(),
      "bdMini":"2",
      "bdMiniList":false,
      "bdPic":"https://s2.51cto.com/images/201710/25/bd540a4f14d822f6e69087758699358b.jpg",
      "bdStyle":"0",
      "bdSize":"16"
    },
    "share":{}
  };

  with(document)0[(getElementsByTagName('head')[0]||body).appendChild(createElement('script')).src='/static/api/js/share.js?v=89860593.js?cdnversion='+~(-new Date()/36e5)];
  setTimeout(function(){
  	$('.bdsharebuttonbox a').removeAttr('title')
  },1000);
  var BLOG_URL=`https://blog.51cto.com/`;


  // 分类列表
  var arr=[]

  var pageNum=0
  var classificationBox=$('#classification_001')
  var addClassification=function(type){
     var classificationHtml="";
     pageNum=pageNum+1;
     var len=type?arr.length:(arr.length<5?arr.length:5)
     for(var i=((pageNum-1)*5);i<len;i++){
      classificationHtml=classificationHtml+'<li class="Classification_648" data-index="'+i+'"> <span class="Classification_648_title" data-index="'+i+'"># '+arr[i].name+'</span> <span>'+arr[i].num+'篇</span></li>'
     }
     classificationBox.append(classificationHtml)
     if(type||arr.length<=5){
      document.getElementById('Classification_648_add').style.display="none"
     }
  }
  document.getElementById("classification_001").addEventListener("click",function(event){
    //  var target = event.target;
     //防止父元素ul也触发事件
     var index=event.target.getAttribute('data-index')
     window.open(`${BLOG_URL}${arr[index].domain}/category${arr[index].custom_id}.html`)
   })
   document.getElementById("Classification_648").style.display="none"
   $.post(BLOG_URL+'blogger/cate-list',{user_id:'',domain:`michaelkang`,blog_user_id:"1553154"},function(res){
    if(res.status===1){
        if(res.data.length>0){
        arr=res.data;
        addClassification()
        document.getElementById("Classification_648").style.display="block"

        }

    }
    })
  addSwiper=function(){
    var arr=$('.swiper-container11')
    var data={}
      for(var i=0;i<arr.length;i++){
       data[`swer${i}`]=new Swiper(arr[i],{
          // loop:true,
          slidesPerView:'auto',
          prevButton:(`.user-perv-${i}`),
          nextButton:(`.user-next-${i}`),
          speed:300,
        //其他设置
       });
      }
    }

    // addSwiper()
</script>
<script>
    var page = 'person';
    var c_user_id ='1553154';
    var nickname = '无锋剑客';
</script>
<div class="dialog-box">
    <div class="mask"></div>
    <div class="body">
        <div id="close" class="close"></div>
        <div id="medalListBox2">
        <script id="medalList2" type="text/html">
            <div class="title">
                <div class="titleP"><span class="txt1">无锋剑客</span> <span class="txt2">（已经获得 {{total}} 枚勋章啦）</span></div>
                <a href="https://blog.51cto.com/creative-center/medal" class="medal-button">勋章管理</a>
            </div>
            <div class="scroll">
                <div class="medal-list">
                    {{each list}}
                    <div class="item">
                        <img src="{{$value.img_light}}">
                        <span class="txt3" title="{{$value.name}}">
                            {{$value.name}}
                            {{if $value.type == 0}}
                             Lv{{$value.level}}</span>
                            {{/if}}
                        <span class="txt4" title="{{$value.rule}}">{{$value.rule}}</span>
                        <span class="txt4">{{$value.get_time}} 获得</span>
                    </div>
                    {{/each}}
                </div>
            </div>
        </script>
        </div>
    </div>
</div></div>
<script src="https://static2.51cto.com/edu/blog/js/template-web.js?v=422383d018"></script><script src="https://static2.51cto.com/edu/blog/blog-static/js/bloger.js?v=c205c57245"></script><script src="https://static2.51cto.com/edu/blog/blog-static/js/share/share.js?v=63a5fd362a"></script><script src="https://static2.51cto.com/edu/blog/js/medal.js?v=c4f6e3b551"></script>
<!-- if publish show -->
<div class="Footer">
  <div class="Page ">
    <div class="fl">
      <a href="https://blog.51cto.com/" class="Logo" ><img src="https://static2.51cto.com/edu/blog/images/logonew4.png" alt="51CTO博客" width="214" title="51CTO博客"></a>
      <p class="copy">Copyright &copy; 2005-2022 <a href="http://www.51CTO.com" target="_blank">51CTO.COM</a>
          版权所有 京ICP证060544号</p>
    </div>

    <dl class="foot_ab fr">
      <dt>关于我们</dt>
      <dd>
        <table class="aboutList">
              <tr>
                  <td><a href="https://blog.51cto.com/51ctoblog" target="_blank">官方博客</a></td>
                  <td><a href="https://blog.51cto.com/51ctoblog/2643377" target="_blank">意见反馈</a></td>
                  <td><a href="http://www.51cto.com/about/aboutus.html" target="_blank">了解我们</a></td>
                  <td><a href="https://blog.51cto.com/nav" target="_blank">全部文章</a></td>
              </tr>
              <tr>
                  <td><a href="javascript:;" class="zhiCustomBtn">在线客服</a></td>
                  <td><a href="http://www.51cto.com/about/map.html" target="_blank">网站地图</a></td>
                  <td><a href="https://blog.51cto.com/topic/all" target="_blank">热门标签</a></td>
              </tr>
          </table>
      </dd>
    </dl>


    <dl class="foot_link fr">
      <dt>友情链接</dt>
      <dd>

        <table class="aboutList-2">
            <tr>
                <td><a href="https://ost.51cto.com/?utm_source=blogsitemap" target="_blank">开源基础软件社区</a></td>
                <td><a href="https://edu.51cto.com/" target="_blank">51CTO学堂</a></td>
            </tr>
            <tr>
              <td><a href="http://www.51cto.com" target="_blank">51CTO</a></td>

            </tr>
        </table>
      </dd>
    </dl>

  </div>
</div>

<script>
  var uid = '';
  var BLOG_URL = 'https://blog.51cto.com/';
</script>
  <script src="//www.sobot.com/chat/frame/js/entrance.js?sysNum=a8d9379eaf884b4f81a48348979e3b1a" id="zhichiScript" class="zhiCustomBtn" data-args="manual=true"></script>
  <script>
      var zhiManager = (getzhiSDKInstance());
      zhiManager.on("load", function() {
          zhiManager.initBtnDOM();
      });
      zhiManager.set('title','欢迎咨询');
      zhiManager.set('powered',false);
      zhiManager.set('color','4285f4');
      zhiManager.set('customBtn', 'true');
      zhiManager.set('size',{'width':360,'height':500});
      zhiManager.set('userinfo', {'partnerId':'','uname':'','params':{'用户名':''}});
      zhiManager.set('customMargin', 20);
      zhiManager.set('preVisitArgs',{'preVisitUrl': document.referrer?document.referrer:''});
      zhiManager.set('curVisitArgs',{'curVisitUrl': location.href,curVisitTitle:document.title,});
  </script>




<script>
    (function(){
        var wh=$(window).height(),fh=$('.Footer').outerHeight(true),hh=$('.Header').outerHeight(true)
        $('.Content-box').css({'min-height': wh-fh-hh})
    })()
</script>
    <div class="zhiCustomBtn" style="display:none;" id="hide-zhiCustomBtn"></div>
</body>
</html>
