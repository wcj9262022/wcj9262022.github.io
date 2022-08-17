Docker大纲：
   1.什么是Docker？
         Docker是一个容器化平台，他以容器的形式将你的应用程序依赖项打包在一起，确保你应用程序在任何环境中无缝运    行 ，我们可以将容器视为Docker镜像运行的实例
 
  2.什么是Docker镜像？
       Docker镜像是Docker容器的源代码，Docker镜像用于创建容器，使用Docker build创建镜像

   3.Docker容器的几种状态？
       运行、停止、重新启动、 已退出

  4.Dockerfile常见指令是？
      FROM     指定基础镜像        【多个FROM 最后一个执行 前面的会被忽略】
     LABEL      功能为镜像指定标签
     WORKDIR    切换路径
    COPY          拷贝文件
     RUN          运行指定命令
     CMD         启动容器时要运行的命令  （CMD指令可被docker  RUN命令覆盖）
     ENTRYPOINT     类似CMD指令，但不会被Docker  RUN命令覆盖 反而这些命令会被当作参数，给ENTRYPOINT，指令指定的程序    【当docker run 使用--entrypoint选项 可覆盖ENTPYPOINT指令】   
           当有多个ENTYRPOINT时最后一个生效

   5.Dockerfile 中COPY和ADD区别
    1>是否支持从远程URL获取资源    COPY只能从本地获取    ADD支持远程获取资源并复制到镜像中 
     2>COPY和ADD本质都是拷贝  但ADD可以在拷贝的时候解压缩文件
     
  6.Dockerfile构建镜像缓慢何解？
     1.减少构建层   eg： 多个run可以融合到一起
     2.写Dockerfile时尽量把不容易出错的写前面  这样每次Dockerfile构建会使用之前build的缓存 大大提高构建速度
      
  7.解释Docker工作流程是什么？
    
