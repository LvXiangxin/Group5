# Group5

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>何以为家：高校毕业生们有着怎样的租房选择？</title>
    <link rel="icon" href="img/house.png">

    <!-- CSS Stylesheets -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet"
        integrity="sha384-0evHe/X+R7YkIZDRvuzKMRqM+OrBnVFBL6DOitfPri4tjfHxaWutUpFmBp4vmVor" crossorigin="anonymous">
    <link rel="stylesheet" href="CSS/style.css">
    <link rel="stylesheet" type="text/css"
        href="https://cdn.jsdelivr.net/gh/bmabey/pyLDAvis@3.3.1/pyLDAvis/js/ldavis.v1.0.0.css">

    <!-- bootstrap scripts -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.bundle.min.js"
        integrity="sha384-pprn3073KE6tl6bjs2QrFaJGz5/SUsLqktiwsUTF55Jfv3qYSDhgCecCxMW52nD2"
        crossorigin="anonymous"></script>

    <!-- 引入 echarts.js -->
    <script src="https://cdn.staticfile.org/echarts/4.3.0/echarts.min.js"></script>
    <script src="https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json"></script>
    <script src="http://libs.baidu.com/jquery/2.0.0/jquery.min.js"></script>
    <script src="echarts-4.2.1-rc1-map_js_china.js"></script>

    <!-- font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+SC&display=swap" rel="stylesheet">


</head>

<body>
    <div data-v-32b84ec5="">
        <!-- /header -->
        <section class="wrapper bg-light">
            <div data-cues="slideInDown" class="container pt-11 pt-md-13 pb-11 pb-md-19 pb-lg-22 text-center">
                <h1 class="display-1 fs-60 mb-4 px-md-15 px-lg-0">何以为家：
                    <br />
                    <span class="c26995">高校毕业生们有着怎样的租房选择？</span>
                </h1>
                <div class="row">
                    <div data-cues="slideInDown" data-group="page-title" class="col-lg-8 col-xl-7 col-xxl-6 mx-auto">
                        <p class="lead lh-sm mb-7 mx-lg-10">
                        <div id="i6wjbh" class="c2111">
                            <br />
                            <br />2022年的毕业季有些不同。除了进阶版的“云毕业”“云面试”，中国高校毕业生数量达到新高。不同的世代、滚动的需求，叠加疫情因素的影响，高校毕业生的居住问题应得到更多关注。
                        </div>
                        <div>
                            <br />
                        </div>
                        </p>
                        <div>
                        </div>
                    </div>
                    <!-- /column -->
                </div>
                <!-- /.row -->
            </div>
            <!-- /.container -->
        </section>
        <!-- /section -->
        <section class="wrapper bg-dark" style="height: 950px;">
            <div class="container py-14 py-md-16">
                <figure data-cue="slideInDown" data-delay="900" class="rounded mt-md-n21 mt-lg-n23 mb-14">
                    <img src="https://static.htmlpage.cn/editor/images/assets/bg8.jpg" class="c28213" />
                </figure>
                <div class="row">
                    <div class="cell">
                        <div data-cues="slideInDown" class="c31570">
                            <h3 id="ifjm57-2" draggable="false" class="display-4 text-white mb-10 gjs-selected c32262">
                                2022年，中国高校毕业生数量首次破千万，规模和增量均创历史新高，这一群体也正式进入到了“00
                                后”时代。对于这群刚刚走出象牙塔的年轻人而言，生活充满着不确定性。繁忙充实的工作用来安放热腾腾的理想，一处温馨舒适的小窝则用来安抚漂泊的心灵。下决心来到大城市打拼，“租房”几乎是这些高校毕业生们人生清单的必选项。面对鱼龙混杂的租房市场，面对各不相同的租房需求，他们都有着怎样的租房选择呢？
                            </h3>
                            <!-- 为ECharts准备一个具备大小（宽高）的Dom 折线图 -->
                            <div id="chart1"></div>
                            <script type="text/javascript">
                                // 基于准备好的dom，初始化echarts实例
                                var myChart1 = echarts.init(document.getElementById('chart1'));
                                var uploadedDataURL = "https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json";

                                let xaxisData = ["2012年", "2013年", "2014年", "2015年", "2016年", "2017年", "2018年", "2019年", "2020年", "2021年", "2022年"];
                                let yaxisData = [680, 699, 727, 749, 756, 795, 820, 834, 874, 909, 1076];
                                let animationData = [["2012年", 680], ["2013年", 699], ["2014年", 727], ["2015年", 749], ["2016年", 756], ["2017年", 795], ["2018年", 820], ["2019年", 834], ["2020年", 874], ["2021年", 909], ["2022年", 1076]]

                                option = {
                                    title: {
                                        text: '2012-2022年全国高校毕业生人数',
                                        top: '4%',
                                        textAlign: 'center',
                                        left: '49.5%',
                                        textStyle: {
                                            color: '#a8d5ff',
                                            fontSize: 22,

                                        },
                                    },
                                    backgroundColor: "#262B32",
                                    grid: {
                                        top: "15%",
                                        left: "1%",
                                        right: "1%",
                                        bottom: "1%",
                                        containLabel: true,
                                    },
                                    tooltip: {
                                        trigger: "axis",
                                        confine: true,
                                        backgroundColor: "rgba(255, 132, 90, 0.3)",
                                        borderColor: "#FF845A",
                                        extraCssText: "box-shadow: 2px 2px 4px 0px rgba(255, 132, 90, 0.3);",
                                        textStyle: {
                                            fontSize: 16,
                                            color: "#fff",
                                            fontFamily: "PangMenZhengDao",
                                        },
                                        formatter: (params, ticket, callback) => {
                                            const item = params[0];
                                            return '毕业生人数' + "<br/>" + item.name + "：" + item.value + " 万人";
                                        },
                                        axisPointer: {
                                            type: "line",
                                            lineStyle: {
                                                color: "#FF845A",
                                            },
                                        },
                                    },
                                    xAxis: {
                                        data: xaxisData,
                                        boundaryGap: true,
                                        axisLine: {
                                            show: true,
                                            symbol: ["none", "rect"],
                                            symbolSize: [6, 12],
                                            lineStyle: {
                                                width: 2,
                                                color: "#537DAA",
                                            },
                                        },
                                        axisTick: {
                                            show: false,
                                        },
                                    },
                                    yAxis: {
                                        name: "(万人)",
                                        nameTextStyle: {
                                            color: "#AEC9FF",
                                            fontWeight: 400,
                                            fontSize: 14,
                                        },
                                        axisLabel: {
                                            color: "#AEC9FF",
                                        },
                                        interval: 100,
                                        min: 500,

                                        axisLine: {
                                            show: true,
                                            symbol: ["none", "rect"],
                                            symbolSize: [6, 12],
                                            lineStyle: {
                                                width: 2,
                                                color: "#537DAA",
                                            },
                                        },
                                        axisTick: {
                                            show: false,
                                        },
                                        splitLine: {
                                            show: true,
                                            lineStyle: {
                                                color: "rgba(83, 125, 170, 0.2)",
                                            },
                                        },
                                    },
                                    series: [
                                        {
                                            type: "line",
                                            // smooth: true,
                                            lineWidth: 1.2,
                                            data: yaxisData,
                                            symbol: "none",
                                            itemStyle: {
                                                color: "rgba(114, 178, 255, 1)",
                                            },
                                            lineStyle: {
                                                width: 5,
                                                shadowBlur: 20,
                                                shadowColor: "#72B2FF",
                                                shadowOffsetY: 10,
                                            },
                                            areaStyle: {
                                                color: new echarts.graphic.LinearGradient(
                                                    0,
                                                    0,
                                                    0,
                                                    1,
                                                    [
                                                        {
                                                            offset: 0,
                                                            color: "rgba(114, 178, 255, 0.25)",
                                                        },
                                                        {
                                                            offset: 1,
                                                            color: "rgba(114, 178, 255, 0)",
                                                        },
                                                    ],
                                                    false
                                                ),
                                                opacity: 1,
                                            },
                                        },
                                        {
                                            type: "lines",
                                            coordinateSystem: "cartesian2d",
                                            data: [{
                                                coords: animationData
                                            }],
                                            zlevel: 1,
                                            polyline: true,
                                            symbol: "circle",
                                            effect:
                                            {
                                                show: true,
                                                trailLength: 0.4,
                                                symbol: "circle",
                                                period: 8,
                                                symbolSize: 8
                                            },
                                            lineStyle:
                                            {
                                                normal:
                                                {
                                                    color: '#64FFFF',
                                                    width: 0,
                                                    opacity: 0,
                                                    curveness: 0
                                                }
                                            }
                                        },
                                    ],
                                };


                                // 使用刚指定的配置项和数据显示图表。
                                myChart1.setOption(option);
                            </script>
                        </div>
                    </div>
                    <div class="cell">
                        <div class="c32496">
                        </div>
                    </div>
                </div>
                <!-- /.row -->
                <!--/.row -->
            </div>
            <!-- /.container -->
        </section>
        <!-- /section -->
        <section class="wrapper bg-light">
            <p align="center" class="MsoNormal c36797">
                <b>
                </b>
                <b>
                </b>
            </p>
            <div class="container py-14 py-md-17">
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/plugins.css" />
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/style.css" />
                <div data-cues="slideInDown" class="c39490">
                    <p align="center" class="MsoNormal c39576">
                        <span><span lang="EN-US" class="c39592"><b id="izrgfa" class="c2475">
                                </b></span></span>
                        <span><span class="c39619">01 入海，就业流向大体趋同<span lang="EN-US">
                                    <o:p>
                                    </o:p>
                                </span></span></span>
                    </p>
                </div>
                <div class="row justify-content-end">
                    <div class="col graduatefloat">
                        <iframe src="图2 毕业生流向地图.html" frameborder="0" style="width: 500px;height: 300px;"></iframe>
                    </div>
                    <div data-cues="slideInDown" class="col col-md-5 text-center">
                        <p class="text-h3">
                        <p class="MsoNormal c41367">
                            <span id="ibwt5o" class="c2584">当应届毕业生面对具体的就业城市时，一线城市因就业机会、经济实力与区位优势较为突出，仍为大部分毕业生工作首选城市。<b>从
                                    <span lang="EN-US">58</span>同城、赶集直招发布的《
                                    <span lang="EN-US">2022</span>年毕业季调研分析报告》来看
                                </b>，北上广深仍为很大一部分毕业生工作首选的就业城市，其中深圳毕业生净流入率达<span
                                    lang="EN-US">3.5%</span>。与此同时，新一线城市也受到了欢迎。<span lang="EN-US">2022</span>年评出的<span
                                    lang="EN-US">15</span>座新一线城市依次是：成都、重庆、杭州、西安、武汉、苏州、郑州、南京、天津、长沙、东莞、宁波、佛山、合肥和青岛。对于应届生而言，为了个人发展，更倾向前往杭州、西安、厦门、长沙、成都、青岛等新一线城市就业。<span
                                    lang="EN-US">2021</span>届本科生中，在新一线城市就业的比例达到<span lang="EN-US">27%</span>，相比<span
                                    lang="EN-US">2017</span>届本科生增加<span
                                    lang="EN-US">3</span>个百分点。同时，选择在一线城市工作的毕业生比例从<span lang="EN-US">2017</span>届的<span
                                    lang="EN-US">22%</span>减少至<span lang="EN-US">2021</span>届的<span
                                    lang="EN-US">18%</span>。<span lang="EN-US">
                                    <o:p>
                                    </o:p>
                                </span></span>
                        </p>
                        </p>
                        <p class="mt-4">
                        </p>
                    </div>
                </div>
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/plugins.css" />
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/style.css" />
                <section
                    data-image-src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/img/map.png"
                    class="wrapper image-wrapper bg-auto no-overlay bg-image text-center bg-map">
                    <!-- /.container -->
                </section>
                <!-- /section -->
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/plugins.js"></script>
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/theme.js"></script>
                <div id="i35m7x" class="row c3253">
                </div>
                <section class="wrapper ";>
                    <!-- /.container -->
                </section>
                <!-- /section -->
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/plugins.js"></script>
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/theme.js"></script>
                <div class="row gx-lg-8 gx-xl-12 gy-10 align-items-center mb-14 mb-md-17">
                    <!--/column -->
                    <!--/column -->
                </div>
                <div data-cues="slideInDown" class="row" style="padding-bottom: 20px;">
                    <div class="cell">
                        <div class="c32141">
                            近年来，在大城市高昂的生活成本、巨大的竞争压力等因素的综合作用下，高校毕业生就业逐渐形成新的发展趋势，越来越多的高校毕业生选择“逆向就业”。麦可思研究院发布的《2022年中国大学生就业报告》显示，近五年大学毕业生就业重心下沉，更多毕业生涌向地级市及以下地区，其民企、政府机关及事业单位对大学生的吸纳能力增强。
                        </div>
                    </div>
                </div>
                <div data-cues="slideInDown" class="row" style="padding-bottom: 180px;">
                    <div class="col cell">
                        <div class="c31297">
                            罗冰是华东政法大学2022届硕士毕业生，毕业后选择留在上海成了一名律师。同为2022届毕业生的张争巍，从南京大学电子与信息科学与工程学院本科毕业后，只身前往深圳打拼。他是苏州人，在深圳除了租房别无选择。在一家名不见经传的小科技公司，为了月度考评能达到S，他每天要工作12-13小时。最早合租在一起的两位室友受不了如此高强度的工作节奏，相继选择了回到苏州、镇江工作。
                        </div>
                    </div>
                    <div class="col cell" id="i6l3ib">
                        <img src="img/luobingimg.png" alt="" style="width: 500px;height: 400px;">
                    </div>
                    <div class="col cell">
                        <div class="c31377">
                            今年31岁的葛慧是南京师范大学法学专业的硕士毕业生。她毕业后没有选择律所，而是在新华日报工作了一段时间，之后成为了一名政府工作人员。从研二就开始租房的她，在南京有过5段租房经验，对于租房有着很积极的态度。在葛慧看来，“租房”是一个非常青春的词，每次租房都给她带来了不同的新鲜体验，能够感受各处不同的人间烟火气息。不同于自己购房之后三点一线的固定生活，租房有一种“永远都在路上”的感觉。
                        </div>
                    </div>
                </div>
                <!--/.row -->
                <!--/.row -->
            </div>
            <div data-cues="slideInDown" class="c31539" >
                对许多高校毕业生而言，毕业后的几年时间是绝佳的“试错”机会。有的人为梦想而坚定地选择只身闯荡，有的人则在体制内外游移不定。面对充满着未知数的未来，租房是他们为自己定制的恒定常数，适应着可能随时发生变化的工作境遇。
            </div>
            <!-- /.container -->
        </section>
        <!-- /section -->
        <section class="wrapper bg-dark" style="margin-top: 60px;height: 1300px;">
            <div data-cues="slideInDown" class="container py-14 pt-md-17 pb-md-21">
                <div class="row gx-lg-8 gx-xl-12 gy-10 gy-lg-0 mb-2 text-white align-items-center">
                    <h3 class="display-4 text-white mb-3 pe-xxl-15">02 徘徊 房屋租赁价格水涨船高
                    </h3>
                    <!-- /column -->
                    <div class="row align-items-center counter-wrapper gy-6 text-center">
                        <div class="c9971">
                            根据2022年ICCRA住房租赁产业研究院发布的《中国住房租赁市场三季度研报》，一线城市仍然是住房租赁行业发展的主力市场，北京、上海、广州和深圳四个城市总计几乎占据了全国住房租赁行业的半壁江山。全国住房平均租金微幅上涨，热点城市租赁住房需求仍然旺盛。
                        </div>
                        <div data-cues="slideInDown" class="col-md-4" id="chart2">
                            <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
                            <div id="chart2"></div>
                            <script type="text/javascript">
                                // 基于准备好的dom，初始化echarts实例
                                var myChart2 = echarts.init(document.getElementById('chart2'));
                                var uploadedDataURL = "https://geo.datav.aliyun.com/areas_v3/bound/100000_full.json";

                                //geoCoordMap把所有可能出现的城市加到数组里面
                                var geoCoordMap = {
                                    北京: [116.405285, 39.904989],
                                    上海: [121.472644, 31.231706],
                                    广州: [113.280637, 23.125178],
                                    深圳: [114.085947, 22.547],

                                    成都: [104.065735, 30.659462],
                                    杭州: [120.153576, 30.287459],
                                    重庆: [106.504962, 29.533155],
                                    西安: [108.948024, 34.263161],
                                    苏州: [120.619585, 31.299379],
                                    武汉: [114.298572, 30.584355],
                                    南京: [118.767413, 32.041544],
                                    天津: [117.190182, 39.125596],
                                    郑州: [113.665412, 34.757975],
                                    长沙: [112.982279, 28.19409],
                                    东莞: [113.760234, 23.048884],
                                    佛山: [113.122717, 23.028762],
                                    宁波: [121.549792, 29.868388],
                                    青岛: [120.369557, 36.094406],
                                    沈阳: [123.429096, 41.796767],
                                };

                                //2015年数据
                                var d1 = {
                                    北京: 39437,
                                    上海: 32324,
                                    广州: 20016,
                                    深圳: 41494,

                                    成都: 7256.67,
                                    杭州: 16080,
                                    重庆: 6289,
                                    西安: 6450,
                                    苏州: 12251,
                                    武汉: 10000,
                                    南京: 18697,
                                    天津: 15553,
                                    郑州: 8790,
                                    长沙: 6448,
                                    东莞: 8371,
                                    佛山: 6082,
                                    宁波: 12250,
                                    青岛: 12384,
                                    沈阳: 7242,
                                };

                                //2016年数据
                                var d2 = {
                                    北京: 57597,
                                    上海: 41741,
                                    广州: 22926,
                                    深圳: 43289,

                                    成都: 7643.42,
                                    杭州: 21655,
                                    重庆: 7493,
                                    西安: 6514,
                                    苏州: 16181,
                                    武汉: 13875,
                                    南京: 24867,
                                    天津: 23220,
                                    郑州: 12091,
                                    长沙: 7601,
                                    东莞: 11651,
                                    佛山: 7161,
                                    宁波: 13857,
                                    青岛: 13523,
                                    沈阳: 7242,
                                };
                                //2017年数据
                                var d3 = {
                                    北京: 57768,
                                    上海: 53195.42,
                                    广州: 28578,
                                    深圳: 51477,

                                    成都: 11269.75,
                                    杭州: 28540,
                                    重庆: 9925,
                                    西安: 8880,
                                    苏州: 15320,
                                    武汉: 16259,
                                    南京: 25733,
                                    天津: 22205,
                                    郑州: 12859,
                                    长沙: 9873,
                                    东莞: 13913,
                                    佛山: 10229,
                                    宁波: 17037,
                                    青岛: 18142,
                                    沈阳: 7999,
                                };
                                //2018年数据
                                var d4 = {
                                    北京: 59868,
                                    上海: 46603,
                                    广州: 32088,
                                    深圳: 53205,

                                    成都: 13252.58,
                                    杭州: 28651,
                                    重庆: 12080,
                                    西安: 12207,
                                    苏州: 16943,
                                    武汉: 17568,
                                    南京: 27568,
                                    天津: 22188,
                                    郑州: 13582,
                                    长沙: 10627,
                                    东莞: 14813,
                                    佛山: 10908,
                                    宁波: 20313,
                                    青岛: 18788,
                                    沈阳: 7242,
                                };
                                //2019年数据
                                var d5 = {
                                    北京: 58568,
                                    上海: 48283.67,
                                    广州: 31692,
                                    深圳: 54790,

                                    成都: 11618.5,
                                    杭州: 27002,
                                    重庆: 11187,
                                    西安: 12446,
                                    苏州: 16818,
                                    武汉: 10000,
                                    南京: 28526,
                                    天津: 20952,
                                    郑州: 13266,
                                    长沙: 10078,
                                    东莞: 16105,
                                    佛山: 12652,
                                    宁波: 22814,
                                    青岛: 16340,
                                    沈阳: 9817,
                                };
                                //2020年数据
                                var d6 = {
                                    北京: 57561,
                                    上海: 51201.83,
                                    广州: 33364,
                                    深圳: 56795,

                                    成都: 12341.08,
                                    杭州: 27851,
                                    重庆: 11275,
                                    西安: 12748,
                                    苏州: 21678,
                                    武汉: 16772,
                                    南京: 28640,
                                    天津: 19729,
                                    郑州: 13509,
                                    长沙: 10151,
                                    东莞: 18296,
                                    佛山: 13173,
                                    宁波: 26075,
                                    青岛: 16619,
                                    沈阳: 10216,
                                };
                                //2021年数据
                                var d7 = {
                                    北京: 58768,
                                    上海: 44812.82,
                                    广州: 35143,
                                    深圳: 57733,

                                    成都: 13304.73,
                                    杭州: 31577,
                                    重庆: 12526,
                                    西安: 13871,
                                    苏州: 22216,
                                    武汉: 16829,
                                    南京: 27977,
                                    天津: 18121,
                                    郑州: 13513,
                                    长沙: 10467,
                                    东莞: 20215,
                                    佛山: 14221,
                                    宁波: 26579,
                                    青岛: 16134,
                                    沈阳: 9999,
                                };

                                var colors = [
                                    ['#1DE9B6', '#F46E36', '#04B9FF', '#5DBD32', '#FFC809', '#FB95D5', '#BDA29A', '#6E7074', '#546570', '#C4CCD3'],
                                    [
                                        '#37A2DA',
                                        '#67E0E3',
                                        '#32C5E9',
                                        '#9FE6B8',
                                        '#FFDB5C',
                                        '#FF9F7F',
                                        '#FB7293',
                                        '#E062AE',
                                        '#E690D1',
                                        '#E7BCF3',
                                        '#9D96F5',
                                        '#8378EA',
                                        '#8378EA',
                                    ],
                                    [
                                        '#DD6B66',
                                        '#759AA0',
                                        '#E69D87',
                                        '#8DC1A9',
                                        '#EA7E53',
                                        '#EEDD78',
                                        '#73A373',
                                        '#73B9BC',
                                        '#7289AB',
                                        '#91CA8C',
                                        '#F49F42',
                                    ],
                                ];
                                var colorIndex = 0;
                                $(function () {
                                    var year = ['2015', '2016', '2017', '2018', '2019', '2020', '2021'];
                                    var mapData = [[], [], [], [], [], [], []];

                                    /*柱子Y名称*/
                                    var categoryData = [];
                                    var barData = [];

                                    for (var key in geoCoordMap) {
                                        mapData[0].push({
                                            year: '2015',
                                            name: key,
                                            value: d1[key],
                                        });
                                        mapData[1].push({
                                            year: '2016',
                                            name: key,
                                            value: d2[key],
                                        });
                                        mapData[2].push({
                                            year: '2017',
                                            name: key,
                                            value: d3[key],
                                        });
                                        mapData[3].push({
                                            year: '2018',
                                            name: key,
                                            value: d4[key],
                                        });
                                        mapData[4].push({
                                            year: '2019',
                                            name: key,
                                            value: d5[key],
                                        });
                                        mapData[5].push({
                                            year: '2020',
                                            name: key,
                                            value: d6[key],
                                        });
                                        mapData[6].push({
                                            year: '2021',
                                            name: key,
                                            value: d7[key],
                                        });
                                    }

                                    for (var i = 0; i < mapData.length; i++) {
                                        mapData[i].sort(function sortNumber(a, b) {
                                            return a.value - b.value;
                                        });
                                        barData.push([]);
                                        categoryData.push([]);
                                        for (var j = 0; j < mapData[i].length; j++) {
                                            barData[i].push(mapData[i][j].value);
                                            categoryData[i].push(mapData[i][j].name);
                                        }
                                    }

                                    $.getJSON(uploadedDataURL, function (geoJson) {
                                        echarts.registerMap('china', geoJson);
                                        var convertData = function (data) {
                                            var res = [];
                                            for (var i = 0; i < data.length; i++) {
                                                var geoCoord = geoCoordMap[data[i].name];
                                                if (geoCoord) {
                                                    res.push({
                                                        name: data[i].name,
                                                        value: geoCoord.concat(data[i].value),
                                                    });
                                                }
                                            }
                                            return res;
                                        };

                                        option = {
                                            backgroundColor: '#f3fffe',
                                            title: {
                                                text: '测试',
                                                textStyle: {
                                                    align: 'center',
                                                    color: '#fff',
                                                    fontSize: 20,
                                                },
                                                top: '5%',
                                                left: 'center',
                                            },
                                            tooltip: {
                                                trigger: 'axis',
                                                axisPointer: {
                                                    lineStyle: {
                                                        color: {
                                                            type: 'linear',
                                                            x: 0,
                                                            y: 0,
                                                            x2: 0,
                                                            y2: 1,
                                                            colorStops: [{
                                                                offset: 0,
                                                                color: 'rgba(0, 255, 233,0)'
                                                            }, {
                                                                offset: 0.5,
                                                                color: 'rgba(255, 255, 255,1)',
                                                            }, {
                                                                offset: 1,
                                                                color: 'rgba(0, 255, 233,0)'
                                                            }],
                                                            global: false
                                                        }
                                                    },
                                                },
                                            },
                                            grid: {
                                                top: '15%',
                                                left: '5%',
                                                right: '5%',
                                                bottom: '15%',
                                                // containLabel: true
                                            },
                                            xAxis: [{
                                                type: 'category',
                                                axisLine: {
                                                    show: true
                                                },
                                                splitArea: {
                                                    // show: true,
                                                    color: '#f00',
                                                    lineStyle: {
                                                        color: '#f00'
                                                    },
                                                },
                                                axisLabel: {
                                                    color: '#fff'
                                                },
                                                splitLine: {
                                                    show: false
                                                },
                                                boundaryGap: false,
                                                data: ['2015', '2016', '2017', '2018', '2019', '2020', '2021'],

                                            }],

                                            yAxis: [{
                                                type: 'value',
                                                min: 0,
                                                // max: 140,
                                                splitNumber: 4,
                                                splitLine: {
                                                    show: true,
                                                    lineStyle: {
                                                        color: 'rgba(255,255,255,0.1)'
                                                    }
                                                },
                                                axisLine: {
                                                    show: false,
                                                },
                                                axisLabel: {
                                                    show: false,
                                                    margin: 20,
                                                    textStyle: {
                                                        color: '#d1e6eb',

                                                    },
                                                },
                                                axisTick: {
                                                    show: false,
                                                },
                                            }],
                                            series: [{
                                                name: '注册总量',
                                                type: 'line',
                                                // smooth: true, //是否平滑
                                                showAllSymbol: true,
                                                // symbol: 'image://./static/images/guang-circle.png',
                                                symbol: 'circle',
                                                symbolSize: 25,
                                                lineStyle: {
                                                    normal: {
                                                        color: "#6c50f3",
                                                        shadowColor: 'rgba(0, 0, 0, .3)',
                                                        shadowBlur: 0,
                                                        shadowOffsetY: 5,
                                                        shadowOffsetX: 5,
                                                    },
                                                },
                                                label: {
                                                    show: true,
                                                    position: 'top',
                                                    textStyle: {
                                                        color: '#6c50f3',
                                                    }
                                                },
                                                itemStyle: {
                                                    color: "#6c50f3",
                                                    borderColor: "#fff",
                                                    borderWidth: 3,
                                                    shadowColor: 'rgba(0, 0, 0, .3)',
                                                    shadowBlur: 0,
                                                    shadowOffsetY: 2,
                                                    shadowOffsetX: 2,
                                                },
                                                tooltip: {
                                                    show: false
                                                },
                                                areaStyle: {
                                                    normal: {
                                                        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [{
                                                            offset: 0,
                                                            color: 'rgba(108,80,243,0.3)'
                                                        },
                                                        {
                                                            offset: 1,
                                                            color: 'rgba(108,80,243,0)'
                                                        }
                                                        ], false),
                                                        shadowColor: 'rgba(108,80,243, 0.9)',
                                                        shadowBlur: 20
                                                    }
                                                },
                                                data: [502.84, 205.97, 332.79, 281.55, 398.35, 214.02,]
                                            },
                                            {
                                                name: '注册总量',
                                                type: 'line',
                                                // smooth: true, //是否平滑
                                                showAllSymbol: true,
                                                // symbol: 'image://./static/images/guang-circle.png',
                                                symbol: 'circle',
                                                symbolSize: 25,
                                                lineStyle: {
                                                    normal: {
                                                        color: "#00ca95",
                                                        shadowColor: 'rgba(0, 0, 0, .3)',
                                                        shadowBlur: 0,
                                                        shadowOffsetY: 5,
                                                        shadowOffsetX: 5,
                                                    },
                                                },
                                                label: {
                                                    show: true,
                                                    position: 'top',
                                                    textStyle: {
                                                        color: '#00ca95',
                                                    }
                                                },

                                                itemStyle: {
                                                    color: "#00ca95",
                                                    borderColor: "#fff",
                                                    borderWidth: 3,
                                                    shadowColor: 'rgba(0, 0, 0, .3)',
                                                    shadowBlur: 0,
                                                    shadowOffsetY: 2,
                                                    shadowOffsetX: 2,
                                                },
                                                tooltip: {
                                                    show: false
                                                },
                                                areaStyle: {
                                                    normal: {
                                                        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [{
                                                            offset: 0,
                                                            color: 'rgba(0,202,149,0.3)'
                                                        },
                                                        {
                                                            offset: 1,
                                                            color: 'rgba(0,202,149,0)'
                                                        }
                                                        ], false),
                                                        shadowColor: 'rgba(0,202,149, 0.9)',
                                                        shadowBlur: 20
                                                    }
                                                },
                                                data: [281.55, 398.35, 214.02, 179.55, 289.57, 356.14,],
                                            },
                                            ]
                                        };
                                        optionXyMap01 = {
                                            timeline: {
                                                data: year,
                                                axisType: 'category',
                                                autoPlay: true,
                                                playInterval: 3000,
                                                left: '10%',
                                                bottom: '3%',
                                                width: '60%',
                                                label: {
                                                    normal: {
                                                        textStyle: {
                                                            color: '#ddd',
                                                        },
                                                    },
                                                    emphasis: {
                                                        textStyle: {
                                                            color: '#fff',
                                                        },
                                                    },
                                                },
                                                symbolSize: 10,
                                                lineStyle: {
                                                    color: '#555',
                                                },
                                                checkpointStyle: {
                                                    borderColor: '#777',
                                                    borderWidth: 2,
                                                },
                                                controlStyle: {
                                                    showNextBtn: true,
                                                    showPrevBtn: true,
                                                    normal: {
                                                        color: '#666',
                                                        borderColor: '#666',
                                                    },
                                                    emphasis: {
                                                        color: '#aaa',
                                                        borderColor: '#aaa',
                                                    },
                                                },
                                            },
                                            baseOption: {
                                                animation: true,
                                                animationDuration: 1000,
                                                animationEasing: 'cubicInOut',
                                                animationDurationUpdate: 1000,
                                                animationEasingUpdate: 'cubicInOut',
                                                grid: {
                                                    right: '1%',
                                                    top: '15%',
                                                    bottom: '10%',
                                                    width: '20%',
                                                },
                                                tooltip: {
                                                    trigger: 'axis', // hover触发器
                                                    axisPointer: {
                                                        // 坐标轴指示器，坐标轴触发有效
                                                        type: 'shadow', // 默认为直线，可选为：'line' | 'shadow'
                                                        shadowStyle: {
                                                            color: 'rgba(150,150,150,0.1)', //hover颜色
                                                        },
                                                    },
                                                },
                                                geo: {
                                                    show: true,
                                                    map: 'china',
                                                    roam: true,
                                                    zoom: 1,
                                                    center: [113.83531246, 34.0267395887],
                                                    label: {
                                                        emphasis: {
                                                            show: true,
                                                        },
                                                    },
                                                    itemStyle: {
                                                        normal: {
                                                            borderColor: 'rgba(147, 235, 248, 1)',
                                                            borderWidth: 1,
                                                            areaColor: {
                                                                type: 'radial',
                                                                x: 0.3,
                                                                y: 0.3,
                                                                r: 0.5,
                                                                colorStops: [
                                                                    {
                                                                        offset: 0,
                                                                        color: 'rgba(147, 235, 248, 0)', // 0% 处的颜色
                                                                    },
                                                                    {
                                                                        offset: 1,
                                                                        color: 'rgba(147, 235, 248, .2)', // 100% 处的颜色
                                                                    },
                                                                ],
                                                                globalCoord: false, // 缺省为 false
                                                            },
                                                            shadowColor: 'rgba(128, 217, 248, 1)',
                                                            // shadowColor: 'rgba(255, 255, 255, 1)',
                                                            shadowOffsetX: -2,
                                                            shadowOffsetY: 2,
                                                            shadowBlur: 10,
                                                        },
                                                        emphasis: {
                                                            areaColor: '#389BB7',
                                                            borderWidth: 0,
                                                        },
                                                    },
                                                },
                                            },
                                            options: [],
                                        };

                                        for (var n = 0; n < year.length; n++) {
                                            optionXyMap01.options.push({
                                                backgroundColor: 'rgb(38,43,50)',
                                                
                                    
                                                title: [
                                                    {
                                                        text: '2015-2021年我国主要城市平均房价',
                                                        left: '20%',
                                                        top: '7%',
                                                        textStyle: {
                                                            color: '#97D8ED',
                                                            fontSize: 18,
                                                        },
                                                    },
                                                    {
                                                        id: 'statistic',
                                                        text: year[n] + '年房价（元/平方米）',
                                                        left: '75%',
                                                        top: '8%',
                                                        textStyle: {
                                                            color: '#97D8ED',
                                                            fontSize: 14,
                                                        },
                                                    },
                                                ],
                                                xAxis: {
                                                    type: 'value',
                                                    scale: true,
                                                    position: 'top',
                                                    min: 0,
                                                    boundaryGap: false,
                                                    splitLine: {
                                                        show: false,
                                                    },
                                                    axisLine: {
                                                        show: true,
                                                    },
                                                    axisTick: {
                                                        show: false,
                                                    },
                                                    axisLabel: {
                                                        margin: 2,
                                                        textStyle: {
                                                            color: '#aaa',
                                                        },
                                                    },
                                                },
                                                yAxis: {
                                                    type: 'category',
                                                    //  name: 'TOP 20',
                                                    nameGap: 16,
                                                    axisLine: {
                                                        show: true,
                                                        lineStyle: {
                                                            color: '#ddd',
                                                        },
                                                    },
                                                    axisTick: {
                                                        show: false,
                                                        lineStyle: {
                                                            color: '#ddd',
                                                        },
                                                    },
                                                    axisLabel: {
                                                        interval: 0,
                                                        textStyle: {
                                                            color: '#ddd',
                                                        },
                                                    },
                                                    data: categoryData[n],
                                                },

                                                series: [
                                                    //地图
                                                    {
                                                        type: 'map',
                                                        map: 'china',
                                                        geoIndex: 0,
                                                        aspectScale: 0.75, //长宽比
                                                        showLegendSymbol: true, // 存在legend时显示
                                                        label: {
                                                            normal: {
                                                                show: true,
                                                            },
                                                            emphasis: {
                                                                show: false,
                                                                textStyle: {
                                                                    color: '#fff',
                                                                },
                                                            },
                                                        },
                                                        roam: true,
                                                        itemStyle: {
                                                            normal: {
                                                                areaColor: '#031525',
                                                                borderColor: '#FFFFFF',
                                                            },
                                                            emphasis: {
                                                                areaColor: '#2B91B7',
                                                            },
                                                        },
                                                        animation: false,
                                                        data: mapData,
                                                    },
                                                    //地图中闪烁的点
                                                    {
                                                        //  name: 'Top 5',
                                                        type: 'effectScatter',
                                                        coordinateSystem: 'geo',
                                                        data: convertData(
                                                            mapData[n]
                                                                .sort(function (a, b) {
                                                                    return b.value - a.value;
                                                                })
                                                                .slice(0, 20)
                                                        ),
                                                        symbolSize: function (val) {
                                                            return val[2] / 6000;
                                                        },
                                                        showEffectOn: 'render',
                                                        rippleEffect: {
                                                            brushType: 'stroke',
                                                        },
                                                        hoverAnimation: true,
                                                        label: {
                                                            normal: {
                                                                formatter: '{b}',
                                                                position: 'right',
                                                                show: false,
                                                            },
                                                        },
                                                        itemStyle: {
                                                            normal: {
                                                                color: colors[colorIndex][n],
                                                                shadowBlur: 10,
                                                                shadowColor: colors[colorIndex][n],
                                                            },
                                                        },
                                                        zlevel: 1,
                                                    },
                                                    //柱状图
                                                    {
                                                        zlevel: 1.5,
                                                        type: 'bar',
                                                        symbol: 'none',
                                                        itemStyle: {
                                                            normal: {
                                                                color: colors[colorIndex][n],
                                                            },
                                                        },
                                                        data: barData[n],
                                                    },
                                                ],
                                            });
                                        }
                                        myChart2.setOption(optionXyMap01);
                                    });
                                });



                                // 使用刚指定的配置项和数据显示图表。
                                myChart2.setOption(option);
                            </script>
                        </div>
                    </div>
                    <div data-cues="slideInDown" class="row">
                        <div class="cell c10691">
                            <div class="c10833">
                                <div class="c10969">
                                    <span id="iwwtnm" class="c3499">
                                        <font color="#ffffff">
                                            在ICCRA长期监测的60个住房租赁企业中，出租房屋的平均月租金达3,162.2元，环比涨幅为0.6%。10个热点城市的住房租赁市场运营情况整体呈现出“租金微幅上涨，出租率小幅下跌的态势。平均租金方面，相比二季度，三季度大部分城市租金水平均呈现小幅上升态势，但涨幅明显收窄，仅上海、成都、北京的增幅超过4%。
                                        </font>
                                    </span>
                                </div>
                            </div>
                        </div>
                        <div class="cell c10700">
                            <div class="c11088">
                                <!-- 为ECharts准备一个具备大小（宽高）的Dom -->
                                <div id="chart3"></div>
                                <script type="text/javascript">
                                    // 基于准备好的dom，初始化echarts实例
                                    var myChart3 = echarts.init(document.getElementById('chart3'));

                                    // 指定图表的配置项和数据
                                    option = {
                                        title: {
                                            text: '2022年全国主要城市租金情况',
                                            top: '8%',
                                            textAlign: 'center',
                                            left: '49.5%',
                                            textStyle: {
                                                color: '#a8d5ff',
                                                fontSize: 18,

                                            },
                                        },
                                        backgroundColor: '#262B32',
                                        animation: true,
                                        grid: {
                                            top: "20%",
                                            bottom: "10%",
                                            right: "5%"
                                        },
                                        tooltip: {
                                            show: true,
                                        },
                                        xAxis: {
                                            data: ['北京', '上海', '深圳', '杭州', '广州', '南京', '成都', '重庆', '西安', '武汉'],
                                            axisLine: {
                                                show: false //隐藏X轴轴线
                                            },
                                            axisTick: {
                                                show: false //隐藏X轴轴线
                                            },
                                            splitLine: {
                                                show: true,
                                                lineStyle: {
                                                    color: "rgba(77, 128, 254, 0.2)",
                                                    width: 2
                                                }
                                            },
                                            axisLabel: {
                                                show: true,
                                                interval: 0,
                                                // margin: 14,
                                                fontSize: 14,
                                                textStyle: {
                                                    color: "#a8d5ff" //X轴文字颜色
                                                }
                                            }
                                        },
                                        yAxis: [
                                            {
                                                name: '单位：元/月/㎡：',
                                                nameTextStyle: {
                                                    color: "#a8d5ff",
                                                    fontSize: 12,
                                                    padding: 10,
                                                },
                                                type: "value",
                                                gridIndex: 0,
                                                min: 0,
                                                max: 120,
                                                interval: 20,
                                                // splitNumber: 4,
                                                splitLine: {
                                                    show: true,
                                                    lineStyle: {
                                                        color: "rgba(77, 128, 254, 0.2)",
                                                        width: 2
                                                    }
                                                },
                                                axisTick: {
                                                    show: false
                                                },
                                                axisLine: {
                                                    show: true,
                                                    lineStyle: {
                                                        color: "rgba(77, 128, 254, 0.2)"
                                                    }
                                                },
                                                axisLabel: {
                                                    show: true,
                                                    margin: 14,
                                                    fontSize: 13,
                                                    textStyle: {
                                                        color: "#a8d5ff"
                                                    }
                                                }
                                            }
                                        ],
                                        series: [
                                            {
                                                name: "城市平均租金",
                                                type: "bar",
                                                barWidth: 16,
                                                itemStyle: {
                                                    normal: {
                                                        label: {
                                                            show: true, //开启显示
                                                            position: 'top', //在上方显示
                                                            textStyle: { //数值样式
                                                                color: '#fff',
                                                                fontSize: 14
                                                            }
                                                        },
                                                        color: new echarts.graphic.LinearGradient(0, 0, 0, 1, [
                                                            {
                                                                offset: 0,
                                                                color: "rgba(146, 225, 255, 1)"
                                                            },
                                                            {
                                                                offset: 1,
                                                                color: "rgba(0, 151, 251, 1)"
                                                            }
                                                        ])
                                                    }
                                                },
                                                data: [118.19, 99.71, 89.56, 72.87, 61.05, 30.34, 38.94, 28.74, 30.21, 40.03],
                                                z: 10,
                                                zlevel: 0
                                            },
                                            {
                                                // 分隔
                                                type: "pictorialBar",
                                                itemStyle: {
                                                    normal: {
                                                        color: "#0F375F"
                                                    }
                                                },
                                                symbolRepeat: "fixed",
                                                symbolMargin: 6,
                                                symbol: "rect",
                                                symbolClip: true,
                                                symbolSize: [18, 2],
                                                symbolPosition: "start",
                                                symbolOffset: [1, 1],
                                                data: [118.19, 99.71, 89.56, 72.87, 61.05, 30.34, 38.94, 28.74, 30.21, 40.03],
                                                width: 2,
                                                z: 0,
                                                zlevel: 1
                                            },
                                            {
                                                name: "外框",
                                                type: "bar",
                                                barGap: "-110%", // 设置外框粗细
                                                data: [100, 100, 100, 100, 100, 100, 100],
                                                barWidth: 16,
                                                itemStyle: {
                                                    normal: {
                                                        color: "transparent", // 填充色
                                                        // barBorderRadius: 0, //圆角半径
                                                        label: {
                                                            // 标签显示位置
                                                            show: false,
                                                            position: "top" // insideTop 或者横向的 insideLeft
                                                        }
                                                    }
                                                },
                                                z: 0
                                            },
                                            {
                                                name: "背影",
                                                type: "line",
                                                smooth: true, //平滑曲线显示
                                                showAllSymbol: false, //显示所有图形。
                                                symbolSize: 0,
                                                lineStyle: {
                                                    width: 0
                                                },
                                                areaStyle: {
                                                    color: "rgba(0, 151, 251, 0.1)"
                                                },
                                                data: [498, 520, 568, 432, 464, 332, 344, 458, 470, 468, 398, 310, 421],
                                                z: 5
                                            }
                                        ],
                                        // dataZoom: [
                                        //   {
                                        //     type: "slider",
                                        //     show: false,
                                        //     xAxisIndex: [0],
                                        //     endValue: 14,
                                        //     startValue: 0
                                        //   }
                                        // ]
                                    }


                                    // 使用刚指定的配置项和数据显示图表。
                                    myChart3.setOption(option);
                                </script>
                            </div>
                        </div>
                    </div>
                    <!-- /.row -->
                </div>
                <!-- /.container -->
        </section>
        <!-- /section -->
        <section class="wrapper bg-light" style="margin-top: 300px;">
            <div class="container py-16 py-md-18">
                <div data-cue="slideInDown" class="card shadow-lg mt-n18 mt-md-n23 mb-14 mb-md-18"
                    style="height: 500px;">
                    <div class="c8334">
                        罗冰目前租住在上海市杨浦区的一个老旧小区，她与同为华东政法大学毕业的校友二人整租一套房屋，个人月租金为3100至3200元（不包含水电费）。这个价格是三季度的全国平均月租金的两倍之多，并且罗冰也坦言，这并非她预期中理想的价格。税前月收入7000元的她将自己的租房预算设置在了2000-2500元这一区间，很可惜，在上海，很难找到同时满足她对于租金、地段、楼层、装修风格四方面要求的出租房屋。
                        <br />
                        <br />
                    </div>
                    <div class="row">

                        <div class="col cell">
                            根据2022年10月和11月安居客全国40城租赁价格分类指数显示，步入四季度之后，整体而言，租赁市场进入需求弱化的淡季，仅一室户型的环比价格表现相对较好。2022年，多座城市受到疫情的影响，招聘市场活跃度持续走低，而由于租赁市场的主力需求为白领上班族，新增需求边际的递减也就导致了租房换房的频率降低。这一现象对合租及改善后的两室、三室挂牌价格的影响更为显著。
                        </div>

                        <div class="col cell c9177">
                            <!-- 2.准备具有大小的DOM容器 薪资占比-->
                            <div class="box"></div>

                            <script src="js/echarts.min.js"></script>
                            <script>
                                //3.初始化实例对象 echarts.init(dom容器)
                                var myChart4 = echarts.init(document.querySelector(".box"));
                                //4.指定配置项和数据
                                var option = {
                                    // 调色盘
                                    // color:["#55aaff","#aaff7f","#55007f","#ffff00"],
                                    // 图表的标题
                                    title: {
                                        text: '高校毕业生租金占薪资比重',
                                        left: 'center',
                                        top: 1,
                                        textStyle: {
                                            color: '#002357'
                                        }
                                    },
                                    tooltip: {
                                        trigger: 'item'
                                    },
                                    legend: {
                                        bottom: '1%',
                                        left: 'center'
                                    },
                                    series: [
                                        {
                                            name: '高校毕业生租金占薪资比重',
                                            type: 'pie',
                                            radius: ['40%', '70%'],
                                            avoidLabelOverlap: false,
                                            itemStyle: {
                                                borderRadius: 5,
                                                borderColor: '#fff',
                                                borderWidth: 2
                                            },
                                            label: {
                                                show: false,
                                                position: 'center'
                                            },
                                            emphasis: {
                                                label: {
                                                    show: true,
                                                    fontSize: 40,
                                                    fontWeight: 'bold'
                                                }
                                            },
                                            labelLine: {
                                                show: false
                                            },
                                            data: [
                                                { value: 11.9, name: '10%以下', itemStyle: { color: '#051181' } },
                                                { value: 45.0, name: '10%-20%', itemStyle: { color: '#0000A1' } },
                                                { value: 30.2, name: '20%-30%', itemStyle: { color: '#1F6ED4' } },
                                                { value: 8.3, name: '30%-40%', itemStyle: { color: '#39BAE8' } },
                                                { value: 9.7, name: '40%以上', itemStyle: { color: '#B9EDF8' } }
                                            ]
                                        }
                                    ]
                                };

                                // 4.3 更新配置
                                myChart4.setOption(option);
		// chart图表，set设置 Option选项  data数据 type类型 bar条（柱状条），series系列（数据） Axis轴线 xAxis水平轴线
		// legend传奇（图例） tooltip 提示 init初始化 document文档 
                            </script>
                        </div>
                        <div class="col cell c9003">
                            罗冰与室友整租的房屋约为50多平米，共有两室一厨一卫，没有一厅，出租方正是将客厅改造成了卧室，属于改善类的两室户型。然而明年，罗冰的室友将面临考公去向的选择问题，一旦室友搬走，罗冰也将随之搬出这里，去寻找一室户型的房屋进行租住。
                        </div>
                    </div>
                    <div class="row gx-0">
                        <div data-image-src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/sandbox/assets/img/photos/tm1.jpg"
                            class="col-lg-6 image-wrapper bg-image bg-cover rounded-top rounded-lg-start">
                        </div>
                        <!--/column -->
                        <div class="col-lg-6">
                            <!--/div -->
                        </div>
                        <!--/column -->
                    </div>
                    <!--/.row -->
                </div>
                <!-- /.card -->
                <!--/.row -->
                <section data-block-type="contents" data-id="2" draggable="true" class="fdb-block">
                    <div data-cues="slideInDown" class="container">
                        <div class="row text-center">
                            <div class="col-12">
                                <h1>
                                    <font color="#60697b" face="Arial Black, Gadget, sans-serif">
                                        <span id="ivd1co"><b>03 权衡，位置、租金、安全和舒适性
                                            </b></span>
                                    </font>
                                </h1>
                                <p class="text-h2">
                                    <em id="ibe3js">
                                        <div class="c12347">
                                            <span id="ibe3js-2" draggable="false" class="gjs-hovered c12355">
                                                <font color="Black"
                                                    face="-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol">
                                                    各城市的租房市场行情的差异、租房需求以及租金承受程度都存在很大的差异，因此高校毕业生在租房时的关注因素各所不同。参与58安居客房产研究院发布的《2022年毕业生租住报告》调研的毕业生中，男、女性分布平均，年龄以95后为主，聚焦在一线和新一线城市，学历覆盖专科及以上。参与调研的毕业生在选择租房时关注因素时，有35%的人选择了交通情况，同时还有34%的人选择了房屋安全性和地理位置，31%也重点关注租金价格。从位置偏好来看，参与的毕业生倾向于选择靠近公司、地铁站和基础设施完善的地区租房。
                                                </font>
                                            </span>
                                        </div>
                                    </em>
                                </p>
                            </div>
                        </div>
                        <div class="row text-center pt-3 pt-xl-5">
                            <img src="https://static.htmlpage.cn/editor/images/assets/bg2.jpg" class="c11944" />
                            <div class="row">
                                <div class="cell">
                                    <div class="row">
                                        <div class="cell">
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div class="col-12 col-sm-10 m-auto m-md-0 col-md-6">
                            </div>
                        </div>
                    </div>
                    <div data-cues="slideInDown" class="row">
                        <div class="col c12853 cell">
                            张争巍是单亲家庭，一同生活的母亲是家政服务人员，对于工作地点要求并不高，于是搬来深圳与张争巍同住。母子二人租下一套两室一厅的小房子，每个月4000元，租期一年，租金由他全额支付。房子面积不大，但终究比之前三人合租的要舒服很多，也自由很多。张争巍优先选择了离公司不远的房源，通勤时间约半小时。对于房子本身，他并没有什么不满，“深圳是一个钱给够了就能很舒服的地方”，除了租金实在太贵——他每天工作到晚上11点的回报仅仅是涨薪2000多元，尚不能覆盖到租金的一半。
                        </div>
                        <div class="col c12993 cell">
                            葛慧在初次租房时把地理位置作为首要因素，她倾向于选择靠近学校的房源。其次，她也面临女生单独在外租房的隐患，因此房屋安全性也是她在租房时着重关注的地方。和葛慧同岁的王雪本科毕业于三峡学院的会计专业，如今在重庆的审计局当一名公务员。她在外的唯一一次租房首先选择了离上班地距离近的房源。尽快协调和适应工作，从学生角色转换到一名公务员是她选择在外租房的第一原因。
                        </div>
                    </div>
                    <div class="row" style="align-items: center;">
                        <div class="cell chart5" style="margin-top: 100px;margin-left: 220px;">
                            <!-- 2.准备具有大小的DOM容器 -->
                            <div data-cues="slideInDown" class="box5"></div>
                            <script src="js/echarts.min.js"></script>
                            <script>
                                //3.初始化实例对象 echarts.init(dom容器)
                                var myChart5 = echarts.init(document.querySelector(".box5"));

                                var option = {
                                    title: {
                                        text: '高校毕业生租房时关注因素',
                                        left: 'center',
                                        top: 20,
                                        textStyle: {
                                            color: '#002357'
                                        }
                                    },
                                    legend: {
                                        top: 'bottom'
                                    },
                                    toolbox: {
                                        show: true,
                                        feature: {
                                            mark: { show: true },
                                            dataView: { show: true, readOnly: true },
                                            restore: { show: true },
                                            saveAsImage: { show: true }
                                        }
                                    },
                                    series: [
                                        {
                                            name: 'Nightingale Chart',
                                            type: 'pie',
                                            radius: [50, 150],
                                            center: ['50%', '50%'],
                                            roseType: 'area',
                                            itemStyle: {
                                                borderRadius: 8
                                            },
                                            data: [
                                                { value: 35, name: '交通情况', itemStyle: { color: '#0024b3' } },
                                                { value: 34, name: '房屋安全性', itemStyle: { color: '#0029cc' } },
                                                { value: 34, name: '地理位置', itemStyle: { color: '#002ee6' } },
                                                { value: 31, name: '租金价格', itemStyle: { color: '#0033ff' } },
                                                { value: 29, name: '租房合同的合规性', itemStyle: { color: '#1a47ff' } },
                                                { value: 27, name: '房屋配套设施', itemStyle: { color: '#335cff' } },
                                                { value: 27, name: '住宅区环境', itemStyle: { color: '#4d70ff' } },
                                                { value: 25, name: '周边配套商业区', itemStyle: { color: '#ffe889' } },
                                                { value: 23, name: '房屋装修情况', itemStyle: { color: '#ffe063' } },
                                                { value: 22, name: '押付方式', itemStyle: { color: '#ffd83a' } },
                                                { value: 17, name: '物业服务', itemStyle: { color: '#ffd427' } },
                                                { value: 16, name: '房型', itemStyle: { color: '#ffd013' } },
                                                { value: 15, name: '户型', itemStyle: { color: '#ffcc00' } }
                                            ]
                                        }
                                    ]
                                };
                                // 4.3 更新配置
                                myChart5.setOption(option);
		// chart图表，set设置 Option选项  data数据 type类型 bar条（柱状条），series系列（数据） Axis轴线 xAxis水平轴线
		// legend传奇（图例） tooltip 提示 init初始化 document文档 
                            </script>
                        </div>
                    </div>
                </section>
                <!--/.row -->
                <!--/.row -->
                <div class="px-lg-5">
                    <!--/.row -->
                    <div class="c12347" style="margin-top: 150px;">
                        <span id="ibe3js-2" draggable="false" class="gjs-hovered c12355">
                            <font color="Black"
                                face="-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif, Apple Color Emoji, Segoe UI Emoji, Segoe UI Symbol">
                                近年来的数据显示,毕业生们愈发关注租住房源的舒适性，而越来越多的00后也开启了“相亲式”租房之旅。后浪研究所的一份报告称，“这届年轻人，租房子和谈恋爱一样认真”。年轻人们对待租房更加挑剔，不再愿意轻易妥协，遇到喜欢的房子要么当机立断，要么就算看上十几套也不将就。从房屋租赁市场来看，2022年集中式长租公寓的租金收入占比高达46%。中国房产经纪公义联合会主席胡景晖认为，这说明集中式租赁住房的租金由于品质、管理、服务的原因较高，也说明90后、00后租客愿意付出更多的租金来获得舒适的租住环境、租住品质；这也反映出未来中高品质的租赁住房将拥有广阔的市场空间和发展前景。
                            </font>
                        </span>
                    </div>
                </div>
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/plugins.css" />
                <link rel="stylesheet"
                    href="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/css/style.css" />
                <section class="wrapper">
                    <div class="container py-14 py-md-16">
                        <section data-block-type="contents" data-id="1" draggable="true" class="fdb-block">
                            <div data-cues="slideInDown" class="container">
                                <div class="row">
                                    <div class="col-12">
                                        <div class="row justify-content-center pb-5">
                                            <div class="col-12 col-lg-8 text-center">
                                                <h1 id="id6dap">
                                                    <h1 id="ibvd52-2" draggable="false" class="gjs-selected">
                                                        <font id="ilvomf-2" draggable="true" color="#60697b"
                                                            face="Arial Black, Gadget, sans-serif">
                                                            <span id="ivd1co-2" draggable="true" class="c24662"><span
                                                                    id="ib318g-2" draggable="true" class="c24670">04
                                                                    吐槽，“努力租到更好的房！”</span></span>
                                                        </font>
                                                    </h1>
                                                </h1>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div data-cues="slideInDown" class="row">
                                <div class="col cell c25275 c25350">
                                    “这世上本没有十全十美的房，但我们可以努力租到更好的房！”是豆瓣“我们在租房生活”小组的口号。
                                    <br />
                                    <br />
                                    <br />该小组建立于2021年，目前已经拥有137765名组员。
                                    <br />
                                    房屋装修的种草物件分享，天花板掉漆、瓷砖脱落、租房合同等问题求助，与房东及室友人际关系、房屋中介雷点的处理探讨……这里是网友们对租房问题进行求助交流、记录分享经验感悟的空间。爬取小组标题后进行统计发现，“租房”“房东”“室友”“合租”“中介”“问题”“转租”等是网友吐槽的热门关键词。引入LDA主题模型处理后，文本共分为六个主题，分别涉及房屋基本设施及环境、租住方式、租房各方关系、租房生活日常等四个主要话题。
                                    <br />
                                    <br />
                                </div>
                                <div class="col cell c25284 c25534">
                                    <img src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/user-upload-images/1064/慈云.jpg"
                                        class="c27234">
                                </div>
                            </div>
                        </section>
                        <div class="row">
                        </div>
                        <!--/.row -->
                    </div>
                    <!-- /.container -->
                </section>
                <!-- /section -->
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/plugins.js"></script>
                <script
                    src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/vip-tpl/assets/js/theme.js"></script>
                <div class="row">
                    <div class="cell">
                        <div class="c26087">
                            <br />
                            <br />
                        </div>
                    </div>
                </div>
                <div data-cues="slideInDown"class="row">
                    <div class="cell" style="margin-top: 30px;">
                        <!-- lda主题词分析 -->
                        <div id="ldavis_el4384816629752812967954054279"></div>
                        <script type="text/javascript">

                            var ldavis_el4384816629752812967954054279_data = { "mdsDat": { "x": [-0.1133120184307694, 0.25494075493098023, -0.11167980968237706, -0.10806613061776499, 0.2536892242443834, 0.21401051715697617, -0.10203902606434136, -0.0986065782273583, -0.09579958430314686, -0.09313734900658166], "y": [-0.2909699743388261, 0.0068951384618273, 0.3882078489633314, -0.013517268966895812, -0.001624340465395172, -0.003418243716324392, -0.018714129758824874, -0.019847286824536816, -0.02418901538174789, -0.02282272797260751], "topics": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10], "cluster": [1, 1, 1, 1, 1, 1, 1, 1, 1, 1], "Freq": [14.772209736671732, 13.960616289785948, 12.808681094730012, 11.716889519971593, 8.708697721824393, 8.471525784599446, 8.317691272735562, 8.200703274543766, 6.565796446873986, 6.477188858263546] }, "tinfo": { "Term": ["\u79df\u623f", "\u5408\u79df", "\u5ba4\u53cb", "\u623f\u4e1c", "\u623f\u5b50", "\u8f6c\u79df", "\u4e2d\u4ecb", "\u623f\u79df", "\u62bc\u91d1", "\u623f\u95f4", "\u6c42\u52a9", "\u79df\u623f\u5b50", "\u516c\u5bd3", "\u79df\u5ba2", "\u5e94\u8be5", "\u4e8c\u623f\u4e1c", "\u7b7e\u5408\u540c", "\u5e2e\u5fd9", "\u670b\u53cb", "\u95ee\u9898", "\u9000\u79df", "\u72ec\u5c45", "\u7535\u8d39", "\u6ce8\u610f", "\u60c5\u4fa3", "\u642c\u5bb6", "\u89e3\u51b3", "\u7a7a\u8c03", "\u6574\u79df", "\u5408\u540c", "\u79df\u623f", "\u9000\u79df", "\u5408\u540c", "\u63d0\u524d", "\u9009\u62e9", "\u751f\u6d3b", "\u566a\u97f3", "\u5206\u4eab", "\u6bd4\u8f83", "\u4fbf\u5b9c", "\u7ecf\u9a8c", "\u505a\u996d", "\u5750\u6807", "\u5230\u5e95", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u77ed\u79df", "\u66f4\u65b0", "\u9a6c\u6876", "\u51fa\u79df", "\u5230\u671f", "\u95ee\u9898", "\u79df\u5230", "\u697c\u4e0a", "\u623f\u4e1c", "\u770b\u623f", "\u642c\u8d70", "\u79df\u91d1", "\u6709\u6ca1\u6709", "\u62bc\u91d1", "\u59d0\u59b9", "\u63a8\u8350", "\u5ba4\u53cb", "\u623f\u4e1c", "\u642c\u8d70", "\u60c5\u51b5", "\u9a6c\u6876", "\u7eed\u79df", "\u7537\u670b\u53cb", "\u5230\u671f", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u51fa\u79df", "\u534a\u591c", "\u9000\u623f", "\u5165\u4f4f", "\u6bd4\u8f83", "\u63d0\u524d", "\u5408\u540c", "\u5408\u79df", "\u5947\u8469", "\u9000\u79df", "\u8981\u6c42", "\u770b\u623f", "\u62bc\u91d1", "\u6d17\u8863\u673a", "\u5395\u6240", "\u81ea\u5982", "\u51b0\u7bb1", "\u5408\u79df", "\u95ee\u9898", "\u60c5\u4fa3", "\u89e3\u51b3", "\u81ea\u5982", "\u770b\u623f", "\u5165\u4f4f", "\u9694\u65ad", "\u6c34\u7535\u8d39", "\u5230\u5e95", "\u5750\u6807", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u51fa\u79df", "\u534a\u591c", "\u9000\u623f", "\u5ba4\u53cb", "\u670b\u53cb", "\u751f\u6d3b", "\u5355\u95f4", "\u6bd4\u8f83", "\u5973\u751f", "\u6574\u79df", "\u5230\u671f", "\u642c\u8d70", "\u820d\u53cb", "\u5408\u540c", "\u59d0\u59b9", "\u5947\u8469", "\u623f\u5b50", "\u642c\u5bb6", "\u6709\u6ca1\u6709", "\u5c0f\u533a", "\u63a8\u8350", "\u51b0\u7bb1", "\u697c\u4e0a", "\u59d0\u59b9", "\u9633\u53f0", "\u51fa\u79df", "\u901a\u52e4", "\u4e2a\u4eba", "\u5904\u7406", "\u5367\u5ba4", "\u665a\u4e0a", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u51fa\u53bb", "\u8bb0\u5f55", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u566a\u97f3", "\u5230\u671f", "\u60c5\u51b5", "\u6bd4\u8f83", "\u516c\u53f8", "\u79df\u5230", "\u9009\u62e9", "\u5165\u4f4f", "\u9694\u97f3", "\u81ea\u5982", "\u9644\u8fd1", "\u5355\u95f4", "\u79df\u623f\u5b50", "\u4e8c\u623f\u4e1c", "\u670b\u53cb", "\u6574\u79df", "\u820d\u53cb", "\u516c\u53f8", "\u6d17\u8863\u673a", "\u5947\u8469", "\u5355\u95f4", "\u8bb0\u5f55", "\u5230\u671f", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u5408\u79df", "\u9644\u8fd1", "\u5408\u540c", "\u751f\u6d3b", "\u642c\u8d70", "\u6bd4\u8f83", "\u63d0\u524d", "\u5c0f\u533a", "\u9000\u79df", "\u566a\u97f3", "\u5ba4\u53cb", "\u9633\u53f0", "\u4e2d\u4ecb", "\u62bc\u91d1", "\u6c42\u52a9", "\u8981\u6c42", "\u79df\u91d1", "\u9000\u623f", "\u7ec8\u4e8e", "\u5230\u671f", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u51fa\u79df", "\u534a\u591c", "\u5165\u4f4f", "\u63d0\u524d", "\u9000\u79df", "\u623f\u4e1c", "\u5408\u540c", "\u60c5\u51b5", "\u642c\u8d70", "\u770b\u623f", "\u95ee\u9898", "\u4e8c\u623f\u4e1c", "\u516c\u53f8", "\u79df\u623f", "\u5408\u7406", "\u566a\u97f3", "\u623f\u5b50", "\u623f\u79df", "\u5206\u4eab", "\u8f6c\u79df", "\u516c\u5bd3", "\u7535\u8d39", "\u7a7a\u8c03", "\u5395\u6240", "\u6b63\u5e38", "\u6c34\u7535", "\u77ed\u79df", "\u51fa\u53bb", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u51fa\u79df", "\u534a\u591c", "\u9000\u623f", "\u5355\u95f4", "\u5165\u4f4f", "\u81ea\u5982", "\u623f\u5b50", "\u6bd4\u8f83", "\u9644\u8fd1", "\u60c5\u51b5", "\u95ee\u9898", "\u5408\u540c", "\u59d0\u59b9", "\u5230\u671f", "\u566a\u97f3", "\u623f\u4e1c", "\u8981\u6c42", "\u5c0f\u533a", "\u623f\u79df", "\u5973\u751f", "\u53d1\u73b0", "\u5408\u9002", "\u9694\u58c1", "\u9694\u97f3", "\u79df\u5230", "\u5408\u79df\u623f", "\u536b\u751f\u95f4", "\u9644\u8fd1", "\u534a\u591c", "\u66f4\u65b0", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u4fbf\u5b9c", "\u6bd4\u8f83", "\u5230\u671f", "\u5165\u4f4f", "\u60c5\u4fa3", "\u63d0\u524d", "\u60c5\u51b5", "\u623f\u5b50", "\u642c\u8d70", "\u9000\u79df", "\u9633\u53f0", "\u770b\u623f", "\u623f\u95f4", "\u5e94\u8be5", "\u7b7e\u5408\u540c", "\u6ce8\u610f", "\u5410\u69fd", "\u5bbd\u5e26", "\u5efa\u8bae", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u51fa\u79df", "\u534a\u591c", "\u9000\u623f", "\u770b\u623f", "\u60c5\u51b5", "\u6709\u6ca1\u6709", "\u5230\u671f", "\u53d1\u73b0", "\u623f\u4e1c", "\u5206\u4eab", "\u6bd4\u8f83", "\u9633\u53f0", "\u79df\u623f", "\u4e8c\u623f\u4e1c", "\u7a7a\u8c03", "\u95ee\u9898", "\u9694\u58c1", "\u5ba4\u53cb", "\u5408\u79df\u623f", "\u79df\u5ba2", "\u5e2e\u5fd9", "\u72ec\u5c45", "\u5408\u7406", "\u75ab\u60c5", "\u53a8\u623f", "\u90bb\u5c45", "\u697c\u4e0b", "\u5e8a\u57ab", "\u5750\u6807", "\u5230\u5e95", "\u505a\u996d", "\u665a\u4e0a", "\u7537\u670b\u53cb", "\u6c34\u7535\u8d39", "\u5367\u5ba4", "\u5904\u7406", "\u4e2a\u4eba", "\u51fa\u53bb", "\u8bb0\u5f55", "\u901a\u52e4", "\u9694\u65ad", "\u7ec8\u4e8e", "\u7eed\u79df", "\u7ecf\u9a8c", "\u77ed\u79df", "\u66f4\u65b0", "\u4fbf\u5b9c", "\u9a6c\u6876", "\u51fa\u79df", "\u751f\u6d3b", "\u9009\u62e9", "\u5408\u540c", "\u5230\u671f", "\u697c\u4e0a", "\u566a\u97f3", "\u5c0f\u533a", "\u6bd4\u8f83", "\u5973\u751f", "\u623f\u4e1c", "\u8981\u6c42", "\u536b\u751f\u95f4", "\u642c\u5bb6"], "Freq": [1749.0, 1569.0, 1469.0, 1325.0, 1066.0, 656.0, 613.0, 522.0, 519.0, 447.0, 397.0, 363.0, 328.0, 289.0, 269.0, 299.0, 260.0, 233.0, 261.0, 309.0, 329.0, 216.0, 234.0, 209.0, 280.0, 267.0, 275.0, 219.0, 217.0, 272.0, 1748.6786410970797, 328.21419899906186, 271.86156603083845, 250.77444087493498, 232.06527689693783, 113.21310229780293, 102.5263708000955, 98.4523161866175, 95.48849015140897, 85.88218142363772, 84.0619667631601, 64.75907021775102, 62.640069163578524, 0.08564753351182805, 0.0856457889649848, 0.08564405828772186, 0.0856502000200641, 0.08564483053000975, 0.08564966397088514, 0.08564955524250362, 0.08564581088875589, 0.08565134345829362, 0.08564928710192043, 0.085647578928248, 0.08564619865862518, 0.08564778959889607, 0.08564554589142659, 0.0856463888267652, 0.08564546582678743, 0.0856461645328362, 0.08565671926957336, 0.08565274873542474, 0.08565154300870774, 0.08564988248016576, 0.08564977395565465, 0.08564909624124921, 0.08564893896735763, 0.08564847462380806, 0.08564823274309642, 0.08564810022280656, 0.08564797586683344, 0.08564790374737108, 1468.867310719938, 1324.5078111797986, 158.9465734693934, 97.20418205964774, 86.15772549504374, 83.88218833824162, 70.61555962654393, 53.08195994237703, 0.08676833517688155, 0.08676859809389725, 0.0867767882889961, 0.08677090141170342, 0.08676843592041582, 0.0867662624321829, 0.08677062376200564, 0.08676962393593818, 0.08676553981462272, 0.08676665295738752, 0.08676558363861273, 0.08676808749454407, 0.08676726609921537, 0.08676658534028106, 0.08676678469549984, 0.08676943064080776, 0.08676660201293664, 0.08676818265019826, 0.08676762404741684, 0.08676890053094431, 0.08677296697971404, 0.08676860822575529, 0.08677564856794691, 0.08677373135538993, 0.08677263309870142, 0.08677184352560352, 0.08677163734343313, 0.08677156291498028, 0.08677118936976456, 0.08677030364462217, 0.08676982369369209, 0.08676979137123536, 0.08676918428567991, 0.08676887193796112, 1568.2786438859948, 308.655267745467, 279.236138317282, 274.67855963979764, 213.64846036706703, 109.24761903269261, 95.14772797952203, 83.13271981325492, 70.6710643483042, 64.06279806450814, 0.088501097532017, 0.0885047176995192, 0.08850194513299431, 0.08850262743196512, 0.08850086064668372, 0.08850021386264292, 0.08849918622909168, 0.08849721495494978, 0.08849840919215175, 0.0884972760010884, 0.08849956884312878, 0.08849999665643833, 0.08849758398132257, 0.08849718159389305, 0.08849766334968545, 0.08849831343770428, 0.0885026130686339, 0.0884968998576056, 0.08849833782264452, 0.08849708769747441, 0.0885053593651222, 0.08850328802697399, 0.08850326428549386, 0.08850208926140268, 0.08850207370124352, 0.08850203238174038, 0.0885017328456957, 0.08850145621481605, 0.08850144190458761, 0.08850090752530997, 0.0885001365122598, 0.08850005954188303, 0.08850003462346863, 1065.8275787198004, 266.66726797302886, 235.26103260809256, 192.2066762588172, 155.9463673913436, 124.01786480702035, 110.07894827365432, 104.81494728236714, 97.54074696050344, 90.55203100219282, 80.00683791435672, 72.34812688537006, 71.31542868787727, 70.73293539323107, 67.58365437434263, 0.09105350042941077, 0.09104735657784314, 0.091043126366427, 0.09104440379308475, 0.09104329885322618, 0.09104560304011414, 0.09104353949795327, 0.09104472054420815, 0.09104539831390289, 0.09104492179384785, 0.09104663608854109, 0.0910439064995856, 0.0910449388440127, 0.09106361126890308, 0.09104664591947657, 0.09106208146212581, 0.091055562343541, 0.09105164109861202, 0.09105138686593434, 0.09105115275663911, 0.09104937971376166, 0.09104872698264284, 0.09104835000110324, 0.0910481720404355, 0.09104723374718582, 0.09104713402698336, 0.0910470825823101, 362.4891674849374, 298.7228224307098, 260.97972100730476, 216.47640284569567, 207.99993552747048, 168.89629511050265, 158.6636648292293, 117.46913073791201, 117.45362434397113, 77.75198937740237, 93.93715488175756, 0.10880271459435786, 0.10880831146048249, 0.10880024531652872, 0.10879768603606686, 0.10880336178944922, 0.10879924309320847, 0.10879840835445302, 0.10879659654829504, 0.10880099454706892, 0.10879711921074824, 0.10879665173404883, 0.10879738779893378, 0.10879735902638239, 0.10879779957516589, 0.10879739278313805, 0.10879453727184245, 0.1087959650984914, 0.10879938395126657, 0.10879624812685831, 0.1088029808160656, 0.10880270866507, 0.10880268967356335, 0.10880133562568174, 0.1088007815770534, 0.10880069633030894, 0.10880057249900839, 0.10879958490222329, 0.10879945079071386, 0.10879943916917828, 0.10879938515075994, 0.10879931971051282, 612.6846059503258, 518.4783911138654, 397.02134001230075, 176.19288265259087, 112.79477522249356, 92.09771953903524, 83.22708613246202, 30.613726702102102, 0.1139092781231215, 0.11390432585555421, 0.11390664215842863, 0.11390203237139662, 0.11390086676143434, 0.1139043301790185, 0.11390362640616915, 0.11390819872122437, 0.11390550995054627, 0.11390370565147968, 0.11390179248067682, 0.11390251644693265, 0.11390630851694099, 0.11390945963516401, 0.11390180526117995, 0.11390727194604694, 0.1139052599262236, 0.1139044437707087, 0.1139020104652634, 0.11390329776528692, 0.11390137959483419, 0.11391238227205817, 0.11392149801700663, 0.11391989365651438, 0.11391781377964655, 0.1139153157915653, 0.11391528994822805, 0.11391508842860514, 0.11391116290554612, 0.11390982168721178, 0.11390952489655726, 0.11390832167210532, 0.11390828417723424, 0.11390782999633972, 0.11390732120929037, 0.11390726488482693, 0.11390694506888922, 0.11390631804313166, 655.5286698413283, 327.07116791212485, 233.846063587379, 218.4185910318497, 153.83926546739755, 134.97999421605584, 100.66813584066179, 85.23675597399576, 77.0482547223025, 0.11016077851763487, 0.11016420739874129, 0.11016622949791921, 0.11016429530803593, 0.11016188898394856, 0.11016559962377537, 0.11016920163919555, 0.11016350643303896, 0.11016545304379376, 0.11016164255706493, 0.11016193063796077, 0.11016386620394593, 0.1101653392442825, 0.11016251443990932, 0.11016572419713674, 0.11016034802432456, 0.11016437053947774, 0.11017113895715656, 0.1101655410893885, 0.11016063889250237, 0.11016168917821516, 0.1101701691899304, 0.1101699460150949, 0.11016910219766783, 0.11016874150664746, 0.11016783377326801, 0.11016740804808173, 0.11016700937033382, 0.11016694490477756, 0.110166801652449, 0.11016663382196426, 0.11016638230487416, 0.11016611924764963, 0.11016600694017029, 0.11016579004246822, 0.11016559332442556, 521.836213723101, 198.692154562681, 179.26895314747287, 161.31212627950208, 159.26533129604738, 131.77708078610556, 112.52497048004541, 110.95806757600606, 110.12285824491934, 95.6586429498346, 91.80581708777865, 85.3930272977767, 0.11322610659651133, 0.11321945125739491, 0.11322482781350045, 0.11322228331027999, 0.1132277014088184, 0.11322011711627629, 0.11323014898032603, 0.11322283050339131, 0.11322018912249758, 0.11321878555041587, 0.11322013396899054, 0.11322140015826798, 0.1132279546823474, 0.11321945540658833, 0.11322126961040568, 0.11322717386941683, 0.11321906190131649, 0.1132304778992314, 0.1132395686425763, 0.11323291500241614, 0.11323274832513405, 0.11323200078344814, 0.11323129543246319, 0.11322707139815577, 0.11322660978453866, 0.1132262604475371, 0.11322525058415744, 0.11322429380203458, 0.11322420398063097, 446.6461644997863, 268.2866724699887, 259.8900089595944, 208.8328703515553, 144.33939118929013, 117.92493108912107, 117.49217569119128, 0.13663945861202229, 0.13663432099893405, 0.1366378223224979, 0.13663970726973185, 0.136632868550171, 0.13663529069999725, 0.13663936755278266, 0.1366382057636098, 0.13663919269452446, 0.13663292010791267, 0.1366343479693245, 0.13664240728228041, 0.13663651948007952, 0.136631294802117, 0.13664466519340868, 0.1366383804535977, 0.13664151827845258, 0.136633561672688, 0.13664877571662457, 0.1366371440260401, 0.13663240059791912, 0.13663219811607594, 0.1366337121425845, 0.13664789706645758, 0.13664595861011114, 0.13664547723240067, 0.13664418858548724, 0.13664336178690795, 0.13664293218984294, 0.13664241970616509, 0.1366421625042137, 0.13664173826872184, 0.13664089161660842, 0.13664041312250974, 0.1366399755144215, 0.13663991129056863, 0.13663960650441023, 0.13663957318238606, 0.13663943420700334, 288.91225950851504, 232.6881997915055, 215.67225075902795, 166.98301708264609, 159.1686446431416, 141.68402418235402, 139.26035703710124, 99.41570729462248, 98.80613514647871, 0.1347105025706982, 0.13470934974826165, 0.134713808764231, 0.13471324795980036, 0.13470581164899553, 0.13471105682132467, 0.13471844565070226, 0.13471683317358654, 0.13470732538075808, 0.13470698259405872, 0.13471379104859524, 0.13470765491681458, 0.13471285484693266, 0.13471199318284696, 0.13471594758285288, 0.13470774767055962, 0.13470587980227952, 0.1347091237078184, 0.1347100607189573, 0.13470904994590482, 0.13470565123985107, 0.13472565631263184, 0.1347192758947165, 0.13471848823958288, 0.134718319079102, 0.13471741736907558, 0.13471698970731258, 0.1347156360574169, 0.13471518408500996, 0.1347145532283672, 0.13471446190393865, 0.13471386833107035, 0.13471206169770195, 0.13471165360163148], "Total": [1749.0, 1569.0, 1469.0, 1325.0, 1066.0, 656.0, 613.0, 522.0, 519.0, 447.0, 397.0, 363.0, 328.0, 289.0, 269.0, 299.0, 260.0, 233.0, 261.0, 309.0, 329.0, 216.0, 234.0, 209.0, 280.0, 267.0, 275.0, 219.0, 217.0, 272.0, 1749.6623983756767, 329.1979736516707, 272.84534986009373, 251.7582235595755, 233.04903240641534, 114.19686327904924, 103.51014610680517, 99.4360699166328, 96.47228231611794, 86.86596746295355, 85.04571579280527, 65.74284442597907, 63.623840935731195, 65.04370151941109, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 86.1959776618761, 86.34918997786751, 87.1403550561219, 91.53036944846532, 178.39281706903648, 309.6361821142662, 113.48113363525911, 111.05729769052328, 1325.4904699310894, 110.22853562762927, 159.9292173969863, 113.75026074190902, 236.23938803176048, 519.43387210207, 105.79329378596455, 156.92470716896545, 1469.8499465362904, 1325.4904699310894, 159.9292173969863, 98.18684228364414, 87.1403550561219, 84.86483270232772, 71.59818321519954, 178.39281706903648, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 91.53036944846532, 92.76196986860108, 93.05319412500833, 96.1286561459888, 96.47228231611794, 251.7582235595755, 272.84534986009373, 1569.2595499986978, 118.42971941027639, 329.1979736516707, 177.14837987313956, 110.22853562762927, 519.43387210207, 159.62424853581172, 154.79848221232518, 214.6293625654713, 124.99620227820552, 1569.2595499986978, 309.6361821142662, 280.21702557401596, 275.65945718528434, 214.6293625654713, 110.22853562762927, 96.1286561459888, 84.1136250917511, 71.65196192063149, 65.04370151941109, 63.623840935731195, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 91.53036944846532, 92.76196986860108, 93.05319412500833, 1469.8499465362904, 261.9403102386946, 114.19686327904924, 118.4142226347132, 96.47228231611794, 199.64832146474834, 217.4369909569094, 178.39281706903648, 159.9292173969863, 208.96051732371134, 272.84534986009373, 105.79329378596455, 118.42971941027639, 1066.8059407331527, 267.6456096371026, 236.23938803176048, 193.1850293949913, 156.92470716896545, 124.99620227820552, 111.05729769052328, 105.79329378596455, 98.51909668222481, 91.53036944846532, 80.98518262227464, 73.32648391551679, 72.29379536061593, 71.7113065454236, 68.56201226210763, 63.623840935731195, 65.04370151941109, 65.74284442597907, 71.59818321519954, 71.65196192063149, 78.00746840411556, 78.7125810305328, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 103.51014610680517, 178.39281706903648, 98.18684228364414, 96.47228231611794, 169.85688648112432, 113.48113363525911, 233.04903240641534, 96.1286561459888, 132.73323933982715, 214.6293625654713, 96.61480708183512, 118.4142226347132, 363.4497511219902, 299.68341776788907, 261.9403102386946, 217.4369909569094, 208.96051732371134, 169.85688648112432, 159.62424853581172, 118.42971941027639, 118.4142226347132, 78.7125810305328, 178.39281706903648, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 1569.2595499986978, 96.61480708183512, 272.84534986009373, 114.19686327904924, 159.9292173969863, 96.47228231611794, 251.7582235595755, 193.1850293949913, 329.1979736516707, 103.51014610680517, 1469.8499465362904, 98.51909668222481, 613.6400806622419, 519.43387210207, 397.9768214248249, 177.14837987313956, 113.75026074190902, 93.05319412500833, 84.1825700060391, 178.39281706903648, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 91.53036944846532, 92.76196986860108, 96.1286561459888, 251.7582235595755, 329.1979736516707, 1325.4904699310894, 272.84534986009373, 98.18684228364414, 159.9292173969863, 110.22853562762927, 309.6361821142662, 299.68341776788907, 169.85688648112432, 1749.6623983756767, 167.91769348985733, 103.51014610680517, 1066.8059407331527, 522.79237961616, 99.4360699166328, 656.4878915295592, 328.03038366252355, 234.80527436227888, 219.3778159927889, 154.79848221232518, 135.9392085029253, 101.62735398497232, 86.1959776618761, 78.00746840411556, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.34918997786751, 86.86596746295355, 87.1403550561219, 91.53036944846532, 92.76196986860108, 93.05319412500833, 118.4142226347132, 96.1286561459888, 214.6293625654713, 1066.8059407331527, 96.47228231611794, 96.61480708183512, 98.18684228364414, 309.6361821142662, 272.84534986009373, 105.79329378596455, 178.39281706903648, 103.51014610680517, 1325.4904699310894, 177.14837987313956, 193.1850293949913, 522.79237961616, 199.64832146474834, 180.22512736437778, 162.2682852058312, 160.2214897881857, 132.73323933982715, 113.48113363525911, 111.91423220762194, 111.07901681565505, 96.61480708183512, 92.76196986860108, 86.34918997786751, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.86596746295355, 96.47228231611794, 178.39281706903648, 96.1286561459888, 280.21702557401596, 251.7582235595755, 98.18684228364414, 1066.8059407331527, 159.9292173969863, 329.1979736516707, 98.51909668222481, 110.22853562762927, 447.57890260011624, 269.2194157710693, 260.8227544508558, 209.76561210483936, 145.27213396181233, 118.85766502194598, 118.42491146649718, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 91.53036944846532, 92.76196986860108, 93.05319412500833, 110.22853562762927, 98.18684228364414, 236.23938803176048, 178.39281706903648, 180.22512736437778, 1325.4904699310894, 99.4360699166328, 96.47228231611794, 98.51909668222481, 1749.6623983756767, 299.68341776788907, 219.3778159927889, 309.6361821142662, 160.2214897881857, 1469.8499465362904, 111.91423220762194, 289.84692745850754, 233.62286615559913, 216.60691814339637, 167.91769348985733, 160.1033121488462, 142.61868932600743, 140.1950166801346, 100.35036766198282, 99.74079486166787, 63.623840935731195, 65.04370151941109, 65.74284442597907, 68.56201226210763, 71.59818321519954, 71.65196192063149, 71.7113065454236, 72.29379536061593, 73.32648391551679, 78.00746840411556, 78.7125810305328, 80.98518262227464, 84.1136250917511, 84.1825700060391, 84.86483270232772, 85.04571579280527, 86.1959776618761, 86.34918997786751, 86.86596746295355, 87.1403550561219, 91.53036944846532, 114.19686327904924, 233.04903240641534, 272.84534986009373, 178.39281706903648, 111.05729769052328, 103.51014610680517, 193.1850293949913, 96.47228231611794, 199.64832146474834, 1325.4904699310894, 177.14837987313956, 111.07901681565505, 267.6456096371026], "Category": ["Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Default", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic1", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic2", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic3", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic4", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic5", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic6", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic7", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic8", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic9", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10", "Topic10"], "logprob": [30.0, 29.0, 28.0, 27.0, 26.0, 25.0, 24.0, 23.0, 22.0, 21.0, 20.0, 19.0, 18.0, 17.0, 16.0, 15.0, 14.0, 13.0, 12.0, 11.0, 10.0, 9.0, 8.0, 7.0, 6.0, 5.0, 4.0, 3.0, 2.0, 1.0, -0.707, -2.3799, -2.5683, -2.649, -2.7266, -3.4443, -3.5435, -3.584, -3.6146, -3.7206, -3.742, -4.0029, -4.0362, -10.6311, -10.6311, -10.6312, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.631, -10.631, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -10.6311, -0.8248, -0.9283, -3.0485, -3.5403, -3.6609, -3.6877, -3.8598, -4.1453, -10.5616, -10.5616, -10.5615, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5615, -10.5616, -10.5615, -10.5615, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -10.5616, -0.6732, -2.2987, -2.3989, -2.4154, -2.6666, -3.3374, -3.4755, -3.6105, -3.7729, -3.8711, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4558, -10.4557, -10.4558, -10.4557, -10.4557, -10.4558, -10.4558, -10.4557, -10.4557, -10.4557, -10.4558, -10.4557, -10.4558, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -10.4557, -0.9704, -2.3559, -2.4812, -2.6833, -2.8924, -3.1215, -3.2407, -3.2897, -3.3616, -3.436, -3.5598, -3.6604, -3.6748, -3.683, -3.7285, -10.3382, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3383, -10.3381, -10.3383, -10.3381, -10.3382, -10.3382, -10.3382, -10.3382, -10.3382, -10.3382, -10.3382, -10.3382, -10.3383, -10.3383, -10.3383, -1.7522, -1.9457, -2.0807, -2.2677, -2.3076, -2.5159, -2.5784, -2.879, -2.8791, -3.2916, -3.1025, -9.8634, -9.8633, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8635, -9.8635, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -9.8634, -1.1997, -1.3667, -1.6336, -2.446, -2.892, -3.0947, -3.196, -4.1961, -9.7899, -9.79, -9.7899, -9.79, -9.79, -9.79, -9.79, -9.7899, -9.7899, -9.79, -9.79, -9.79, -9.7899, -9.7899, -9.79, -9.7899, -9.7899, -9.79, -9.79, -9.79, -9.79, -9.7899, -9.7898, -9.7898, -9.7898, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -9.7899, -1.1138, -1.8091, -2.1446, -2.2128, -2.5633, -2.6941, -2.9874, -3.1538, -3.2548, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.8051, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -9.805, -1.3277, -2.2933, -2.3962, -2.5017, -2.5145, -2.704, -2.8619, -2.8759, -2.8835, -3.0243, -3.0654, -3.1378, -9.7634, -9.7635, -9.7634, -9.7635, -9.7634, -9.7635, -9.7634, -9.7635, -9.7635, -9.7635, -9.7635, -9.7635, -9.7634, -9.7635, -9.7635, -9.7634, -9.7635, -9.7634, -9.7633, -9.7634, -9.7634, -9.7634, -9.7634, -9.7634, -9.7634, -9.7634, -9.7634, -9.7635, -9.7635, -1.261, -1.7707, -1.8025, -2.0212, -2.3906, -2.5927, -2.5963, -9.3531, -9.3532, -9.3531, -9.3531, -9.3532, -9.3532, -9.3531, -9.3531, -9.3531, -9.3532, -9.3532, -9.3531, -9.3532, -9.3532, -9.3531, -9.3531, -9.3531, -9.3532, -9.3531, -9.3531, -9.3532, -9.3532, -9.3532, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -9.3531, -1.683, -1.8994, -1.9754, -2.2312, -2.2792, -2.3955, -2.4128, -2.7498, -2.756, -9.3538, -9.3538, -9.3537, -9.3537, -9.3538, -9.3538, -9.3537, -9.3537, -9.3538, -9.3538, -9.3537, -9.3538, -9.3537, -9.3537, -9.3537, -9.3538, -9.3538, -9.3538, -9.3538, -9.3538, -9.3538, -9.3536, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3537, -9.3538], "loglift": [30.0, 29.0, 28.0, 27.0, 26.0, 25.0, 24.0, 23.0, 22.0, 21.0, 20.0, 19.0, 18.0, 17.0, 16.0, 15.0, 14.0, 13.0, 12.0, 11.0, 10.0, 9.0, 8.0, 7.0, 6.0, 5.0, 4.0, 3.0, 2.0, 1.0, 1.9119, 1.9094, 1.9088, 1.9085, 1.9082, 1.9038, 1.9029, 1.9025, 1.9022, 1.901, 1.9008, 1.8973, 1.8968, -4.7202, -4.7729, -4.8162, -4.8169, -4.8178, -4.8258, -4.84, -4.9019, -4.9109, -4.9393, -4.9773, -4.9781, -4.9861, -5.0017, -5.0035, -5.0126, -5.0618, -5.729, -6.2804, -5.2767, -5.2551, -7.7346, -5.2476, -5.6198, -5.2791, -6.0099, -6.7978, -5.2066, -5.6009, 1.9683, 1.9682, 1.9628, 1.9589, 1.9576, 1.9573, 1.9551, 0.7568, -4.6286, -4.6506, -4.6612, -4.7033, -4.7474, -4.7483, -4.7563, -4.7705, -4.8324, -4.8414, -4.8699, -4.9078, -4.9086, -4.9188, -4.9322, -4.934, -4.94, -4.9923, -5.0056, -5.0087, -5.0412, -5.0448, -6.004, -6.0844, -7.8339, -5.2499, -6.2722, -5.6525, -5.1781, -6.7283, -5.5484, -5.5177, -5.8445, -5.3039, 2.0544, 2.0519, 2.0515, 2.0515, 2.0505, 2.0461, 2.0448, 2.0433, 2.0413, 2.0399, -4.5227, -4.5554, -4.5974, -4.6407, -4.6423, -4.6504, -4.6646, -4.7265, -4.7355, -4.764, -4.8027, -4.8108, -4.8129, -4.8264, -4.8281, -4.8341, -4.8372, -4.8864, -4.8998, -4.9029, -7.6626, -5.9378, -5.1076, -5.1439, -4.9389, -5.6662, -5.7516, -5.5537, -5.4444, -5.7118, -5.9786, -5.0312, -5.144, 2.1432, 2.1405, 2.14, 2.1391, 2.1379, 2.1363, 2.1353, 2.1348, 2.1342, 2.1334, 2.132, 2.1307, 2.1305, 2.1304, 2.1298, -4.4052, -4.4273, -4.438, -4.5233, -4.5241, -4.6091, -4.6181, -4.6844, -4.6852, -4.6933, -4.6954, -4.7089, -4.7107, -4.7164, -4.7198, -4.8917, -5.4361, -4.8391, -4.8214, -5.3872, -4.9839, -5.7035, -4.8179, -5.1406, -5.6212, -4.823, -5.0264, 2.4382, 2.4376, 2.4372, 2.4364, 2.4362, 2.4352, 2.4348, 2.4327, 2.4327, 2.4286, 1.7995, -3.9304, -3.9524, -3.9631, -4.0052, -4.0484, -4.0492, -4.0501, -4.0582, -4.0723, -4.1342, -4.1717, -4.2096, -4.2104, -4.2185, -4.2206, -4.2341, -4.2358, -4.2418, -4.245, -7.1357, -4.3481, -5.3863, -4.5153, -4.8521, -4.3466, -5.3059, -5.041, -5.5741, -4.4171, -7.0703, -4.3677, 2.4669, 2.4666, 2.4661, 2.4631, 2.46, 2.4581, 2.457, 0.7059, -3.8569, -3.879, -3.8897, -3.9317, -3.975, -3.9758, -3.9766, -3.9846, -3.9988, -4.0607, -4.0698, -4.0982, -4.1361, -4.145, -4.1471, -4.1605, -4.1623, -4.1683, -4.1715, -4.2206, -4.234, -4.2696, -5.2323, -5.5005, -6.8934, -5.3127, -4.2907, -4.7786, -4.4064, -5.4393, -5.4066, -4.8389, -7.1711, -4.8274, -4.3436, -6.6763, -5.9631, -4.3034, 2.4853, 2.4839, 2.4827, 2.4824, 2.4806, 2.4797, 2.4773, 2.4756, 2.4744, -3.872, -3.8941, -3.9047, -3.9467, -3.9901, -3.9908, -3.9916, -3.9997, -4.0139, -4.0848, -4.1133, -4.1512, -4.152, -4.1601, -4.1622, -4.1774, -4.1834, -4.1865, -4.2357, -4.2491, -4.2522, -4.4931, -4.2846, -5.0879, -6.6914, -4.2882, -4.2897, -4.3058, -5.4544, -5.3279, -4.3805, -4.903, -4.3587, -6.9085, -4.896, -4.9826, 2.4991, 2.4961, 2.4956, 2.495, 2.495, 2.4937, 2.4925, 2.4924, 2.4923, 2.491, 2.4906, 2.4898, -3.8304, -3.8525, -3.8632, -3.9052, -3.9485, -3.9493, -3.95, -3.9582, -3.9724, -4.0343, -4.0433, -4.0717, -4.1096, -4.1105, -4.1185, -4.1206, -4.1341, -4.1417, -4.2466, -4.8613, -4.243, -5.3129, -5.2058, -4.2643, -6.6498, -4.7521, -5.4741, -4.2677, -4.38, 2.7212, 2.7198, 2.7197, 2.7188, 2.7169, 2.7154, 2.7154, -3.4201, -3.4422, -3.4529, -3.4948, -3.5382, -3.539, -3.5398, -3.5479, -3.562, -3.624, -3.633, -3.6614, -3.6993, -3.7002, -3.7081, -3.7103, -3.7237, -3.7256, -3.7314, -3.7347, -3.7838, -3.7972, -3.8003, -3.9696, -3.8539, -4.7319, -4.4511, -4.4613, -6.4566, -3.8666, -3.8363, -3.8573, -6.7343, -4.9698, -4.6579, -5.0025, -4.3437, -6.56, -3.9848, 2.7337, 2.7329, 2.7326, 2.7313, 2.731, 2.7303, 2.7302, 2.7275, 2.7275, -3.4207, -3.4428, -3.4535, -3.4955, -3.5388, -3.5396, -3.5403, -3.5484, -3.5627, -3.6246, -3.6335, -3.662, -3.6999, -3.7007, -3.7088, -3.711, -3.7244, -3.7262, -3.7321, -3.7353, -3.7845, -4.0056, -4.7189, -4.8766, -4.4517, -3.9777, -3.9074, -4.5314, -3.837, -4.5643, -6.4573, -4.4447, -3.978, -4.8574] }, "token.table": { "Topic": [4, 6, 5, 1, 1, 3, 5, 7, 4, 7, 4, 1, 3, 2, 5, 6, 8, 5, 4, 8, 7, 10, 8, 1, 10, 3, 8, 8, 9, 1, 1, 4, 5, 8, 4, 2, 9, 4, 10, 10, 9, 9, 3, 2, 2, 4, 8, 9, 6, 4, 1, 4, 2, 5, 4, 8, 4, 5, 4, 10, 7, 1, 7, 3, 6, 9, 5, 10, 1, 7, 2, 10, 3, 7, 8, 10, 1, 5, 6, 7, 9, 6, 1, 2, 3, 5, 6, 3, 5, 7, 6, 1, 1, 4, 10, 3, 4, 8, 8, 3, 8, 2], "Freq": [0.9819098933334224, 0.9989569119058339, 0.9977195342572528, 0.990030992709281, 0.9887007562197061, 0.9882589001943943, 0.9949552443891079, 0.9968588773667271, 0.9920301396358566, 0.9870849750065418, 0.9942055358056439, 0.9855578572459993, 0.9839538418781469, 0.2970971638364198, 0.5269270452947823, 0.1737738128099814, 0.9917857515350263, 0.9880569867094781, 0.9900809707744895, 0.9902860427955914, 0.994841795598293, 0.995661933727401, 0.993202238875932, 0.9969017252427897, 0.9945348612717053, 0.9991973603100271, 0.99183095671044, 0.9921840228716139, 0.9912430971644793, 0.9950715352456485, 0.9901948557874498, 0.9821036459054028, 0.9879276973938999, 0.9967526826171549, 0.9925014737931357, 0.9994217460508175, 0.9927841000259628, 0.9938658321573751, 0.9973338818847284, 0.9925727996985056, 0.9954705504148845, 0.9879678063605706, 0.9956568464334995, 0.987912410094465, 0.9996299709864267, 0.999244529204066, 0.9984843321229323, 0.9987065909569168, 0.9972395483254348, 0.9941073194549932, 0.9969882868219553, 0.9975878190642544, 0.9941898208963298, 0.9933912304866555, 0.9918028622036487, 0.9843751866321696, 0.9947536774367454, 0.9964102117851286, 0.9904797099109183, 0.9865434707072389, 0.9930909668132641, 0.9847388049627187, 0.9938269180454596, 0.9909009899637686, 0.9975455318696006, 0.9963501543596349, 0.9960892624927743, 0.9971980666702687, 0.9895192981253381, 0.9965704588005275, 0.9916452738276668, 0.9931087487570498, 0.9888546498360509, 0.9861249017144674, 0.9957602323853626, 0.9970780181596758, 0.9996214136073955, 0.9960111373924051, 0.993404316288898, 0.9937194379178513, 0.9968455418984127, 0.9859523176121344, 0.9877040744138962, 0.9898092923206341, 0.9970676772369423, 0.9954033549686166, 0.9935174124992735, 0.9976077106440753, 0.9909470503799591, 0.9992568156460244, 0.98868180576807, 0.9963609324857562, 0.9954986622532467, 0.9878350262310371, 0.9914760402442755, 0.9979453883266413, 0.994731004447806, 0.9936365128658347, 0.9923762424765834, 0.9867604672782042, 0.9944758423475984, 0.9869135826289959], "Term": ["\u4e2a\u4eba", "\u4e2d\u4ecb", "\u4e8c\u623f\u4e1c", "\u4fbf\u5b9c", "\u505a\u996d", "\u5165\u4f4f", "\u516c\u53f8", "\u516c\u5bd3", "\u51b0\u7bb1", "\u51fa\u53bb", "\u51fa\u79df", "\u5206\u4eab", "\u5230\u5e95", "\u5230\u671f", "\u5230\u671f", "\u5230\u671f", "\u534a\u591c", "\u5355\u95f4", "\u5367\u5ba4", "\u536b\u751f\u95f4", "\u5395\u6240", "\u53a8\u623f", "\u53d1\u73b0", "\u5408\u540c", "\u5408\u7406", "\u5408\u79df", "\u5408\u79df\u623f", "\u5408\u9002", "\u5410\u69fd", "\u566a\u97f3", "\u5750\u6807", "\u5904\u7406", "\u5947\u8469", "\u5973\u751f", "\u59d0\u59b9", "\u5ba4\u53cb", "\u5bbd\u5e26", "\u5c0f\u533a", "\u5e2e\u5fd9", "\u5e8a\u57ab", "\u5e94\u8be5", "\u5efa\u8bae", "\u60c5\u4fa3", "\u60c5\u51b5", "\u623f\u4e1c", "\u623f\u5b50", "\u623f\u79df", "\u623f\u95f4", "\u62bc\u91d1", "\u63a8\u8350", "\u63d0\u524d", "\u642c\u5bb6", "\u642c\u8d70", "\u6574\u79df", "\u665a\u4e0a", "\u66f4\u65b0", "\u6709\u6ca1\u6709", "\u670b\u53cb", "\u697c\u4e0a", "\u697c\u4e0b", "\u6b63\u5e38", "\u6bd4\u8f83", "\u6c34\u7535", "\u6c34\u7535\u8d39", "\u6c42\u52a9", "\u6ce8\u610f", "\u6d17\u8863\u673a", "\u72ec\u5c45", "\u751f\u6d3b", "\u7535\u8d39", "\u7537\u670b\u53cb", "\u75ab\u60c5", "\u770b\u623f", "\u77ed\u79df", "\u79df\u5230", "\u79df\u5ba2", "\u79df\u623f", "\u79df\u623f\u5b50", "\u79df\u91d1", "\u7a7a\u8c03", "\u7b7e\u5408\u540c", "\u7ec8\u4e8e", "\u7ecf\u9a8c", "\u7eed\u79df", "\u81ea\u5982", "\u820d\u53cb", "\u8981\u6c42", "\u89e3\u51b3", "\u8bb0\u5f55", "\u8f6c\u79df", "\u9000\u623f", "\u9000\u79df", "\u9009\u62e9", "\u901a\u52e4", "\u90bb\u5c45", "\u95ee\u9898", "\u9633\u53f0", "\u9644\u8fd1", "\u9694\u58c1", "\u9694\u65ad", "\u9694\u97f3", "\u9a6c\u6876"] }, "R": 30, "lambda.step": 0.01, "plot.opts": { "xlab": "PC1", "ylab": "PC2" }, "topic.order": [10, 2, 9, 4, 1, 6, 8, 7, 3, 5] };

                            function LDAvis_load_lib(url, callback) {
                                var s = document.createElement('script');
                                s.src = url;
                                s.async = true;
                                s.onreadystatechange = s.onload = callback;
                                s.onerror = function () { console.warn("failed to load library " + url); };
                                document.getElementsByTagName("head")[0].appendChild(s);
                            }

                            if (typeof (LDAvis) !== "undefined") {
                                // already loaded: just create the visualization
                                !function (LDAvis) {
                                    new LDAvis("#" + "ldavis_el4384816629752812967954054279", ldavis_el4384816629752812967954054279_data);
                                }(LDAvis);
                            } else if (typeof define === "function" && define.amd) {
                                // require.js is available: use it to load d3/LDAvis
                                require.config({ paths: { d3: "https://d3js.org/d3.v5" } });
                                require(["d3"], function (d3) {
                                    window.d3 = d3;
                                    LDAvis_load_lib("https://cdn.jsdelivr.net/gh/bmabey/pyLDAvis@3.3.1/pyLDAvis/js/ldavis.v3.0.0.js", function () {
                                        new LDAvis("#" + "ldavis_el4384816629752812967954054279", ldavis_el4384816629752812967954054279_data);
                                    });
                                });
                            } else {
                                // require.js not available: dynamically load d3 & LDAvis
                                LDAvis_load_lib("https://d3js.org/d3.v5.js", function () {
                                    LDAvis_load_lib("https://cdn.jsdelivr.net/gh/bmabey/pyLDAvis@3.3.1/pyLDAvis/js/ldavis.v3.0.0.js", function () {
                                        new LDAvis("#" + "ldavis_el4384816629752812967954054279", ldavis_el4384816629752812967954054279_data);
                                    })
                                });
                            }
                        </script>
                    </div>
                </div>

                <div data-cues="slideInDown" data-block-type="contents" data-id="10" draggable="true"
                    class="fdb-block pb-0 fp-active c29990" style="margin-top: 800px;">
                    <div class="container">
                        <div class="row text-left justify-content-end">
                            <div class="box6">

                                <div>
                                    关于租房环境，本科毕业的纪玉潇在与女友合租期间就曾两次遭遇房屋安全问题。他们第一次选择的租房是青年公寓，但在居住期间女友的衣物竟遭遇偷窃，衣物在被弄脏后又被还回。两人立刻报了警并联系房东调楼道监控。即使在入住之前，房东向他们保证每一层楼和天台都安装了监控，但找到房东之后，房东却告诉他们天台能够拍摄到“小偷”的两个监控都坏掉了，这也导致了没有直接证据的僵局。在此情况下，他们尝试自己去蹲点“小偷”，找到了
                                    “小偷”本人。最终“小偷”被判定为毁坏公私罪。
                                </div>
                                <div>
                                    有了第一次租房的经验，在第二次租房时，他们特别关注并向中介表达了对租房的安全性的高要求，但这次租房他们仍遇到了“偷电”的问题。在0.85块一度的阶梯电价的情况下，他们发现不到一个周的时间，充的一百块钱电费居然已经花光了，在刻意节省用电的情况下，十几天内就已经充了两百多块钱电费了。在断电实验后，两人发现对门的一家走出门拉上了他们关掉的电闸，也就是说，邻居家的一部分用电都是接在他们家的，两人一起付了双倍的电费。经过沟通，他们发现邻居家并不是故意用他们的电，而是对房屋内的改装线路并不知情。因此纪玉潇在与女友希望由房东来出面协商赔偿，但至今没有得到妥善处理。在谈及两段维权事件时，纪玉潇作为过来人给出了毕业生在外租房建议：“在外面，你不要因为自己是高校的学生，素质高，所以显得好欺负，在有些时候还是需要‘刚’一点，才能有力地保护自己的权益”。
                                </div>
                                <div>
                                    <br />
                                </div>
                                </p>
                            </div>
                            <div class="col-12 col-md-6 col-xl-4">
                            </div>
                        </div>
                    </div>
                </div>


                <section data-block-type="contents" data-id="9" draggable="true" class="fdb-block pb-0 c28877">
                    <div data-cues="slideInDown" class="container">
                        <div class="row text-left">
                            <div class="col-12 col-md-8 col-lg-6">
                                <div class="box6">
                                    <h2>
                                    </h2>
                                    <p class="text-h3">
                                        租房中介也频频爆雷。罗冰是通过租房软件“自如”APP找到房源的，自如公司的服务态度给罗冰带来了糟糕的体验。第一个问题是自如的服务费太高，她和室友两个人算下来每个月需要缴纳
                                        500
                                        元的服务费。对接到它所提供的基本服务，实际上就是每月的一套全屋保洁，而保洁人员前来工作的时间也并不固定，常常错开她或室友居家的时间。第二个问题是自如管家的服务态度欠佳，她与室友在自如管家建立的微信群中上报的问题常常得不到及时的解决，反而像皮球一样被踢来踢去。例如，原本包含在合同中的小区门禁卡，自如提供的两张卡均不能使用，最终两人去了门卫室自费办理。此外，她们在“自如”APP找不到投诉的方式，“合同应该是一直在履行过程中，他们的履约态度实在是让人难以恭维。”
                                    </p>
                                </div>
                            </div>
                        </div>
                    </div>
                </section>
                <!-- /div -->
            </div>
            <!-- /.container -->
        </section>
        <!-- /section -->
    </div>
    <!-- /.content-wrapper -->
    <footer class="bg-navy text-inverse">
        <div data-cues="slideInDown" class="container pt-15 pt-md-17 pb-13 pb-md-15">
            <h3 class="display-4 mb-6 mb-lg-0 pe-lg-20 pe-xl-22 pe-xxl-25 text-white">05 回望，在租房与买房中拉扯的青春
            </h3>
            <div class="d-lg-flex flex-row align-items-lg-center">
            </div>
            <!--/div -->
            <hr class="mt-11 mb-12" />
            <section data-block-type="contents" data-id="9" draggable="true" class="fdb-block pb-0 c16882">
                <div data-cues="slideInDown" class="container">
                    <div class="row text-left">
                        <div class="row">
                        </div>
                        <div class="col-12 col-md-8 col-lg-6">
                        </div>
                        <div class="box6">
                            <p class="text-h3">
                            <div>买房或许并非每一个都市漂泊者的终极归宿。有的人就像王家卫《阿飞正传》中的无脚鸟，终身飞翔，在旅途中纵情享乐，无拘无束。
                            </div>
                            <div>罗冰便梦想着成为“无脚鸟”，目前还在为自己的“Fire计划”攒钱。所谓“Fire计划”，是“the Financial Independence,
                                Retire Early movement”
                                的缩写，即“财务独立，提早退休”。准备不婚不育、没有恋爱打算的她不存在买婚房或者学区房的刚需，而是更倾向于在一个经济实惠且热闹的地方买房。在罗冰未来十年的规划里，能全款买下两套房是最理想的状态：一套在家乡；另一套在云南大理或丽江——那是她最向往的旅居地。当然，如果房价实在太高，超出她的支付能力，她也愿意一直租房。
                            </div>
                            </p>
                            <p class="text-h3 mt-4">
                            </p>
                        </div>
                        <div class="c18293">
                        </div>
                    </div>
                </div>
            </section>
            <section data-block-type="contents" data-id="4" draggable="true" class="fdb-block pt-0 pb-0">
                <div class="col-fill-right c19181">
                </div>
            </section>
            <div class="row">
                <div class="cell">
                    <div class="row">
                        <div class="cell">
                            <div class="row">
                                <div class="cell">
                                    <div class="row">
                                        <div class="cell">
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <section data-block-type="contents" data-id="10" draggable="true" class="fdb-block pb-0 fp-active c20011">
                <div data-cues="slideInDown" class="container">
                    <div class="row text-left justify-content-end">
                        <div class="col-12 col-md-6 col-xl-4">
                            <div class="box6">
                                <h2>
                                    <strong></strong>
                                </h2>
                                <p class="text-h3">
                                    人们年少时大多冒出过“攒够钱就去环游世界“的想法，可真正有勇气付诸实践的终究是少数。真正踏上工作岗位后，也就务实地进入了既定的人生轨道。王雪已经和父母凑钱买下一套学区房，尽管她暂时还没有男朋友。房子没有装修，也没有家具。主城区有更好的初高中教育资源，这是对未来的投资。现在的王雪住在父母家里，计划着房子的装修事宜。
                                </p>
                            </div>
                        </div>
                    </div>
                </div>
            </section>
            <div data-cues="slideInDown" class="row">
                <div class="cell">
                    <div class="row">
                        <div class="cell">
                            <div class="c20900">
                                <div>
                                    <b>介于两种情况中间的，是更多更多高校毕业生的无奈选择：
                                        <br />没有勇气踏上旅途，没有能力拿下住宅；
                                        <br />在折叠的城市里忙碌着积攒未来资本，在租赁的房屋里享受着微小私人空间；
                                        <br />这或许是大多数人的真实写照。
                                    </b>
                                </div>
                                <div>
                                    <b>无论选择哪条路，租房是无可避免的过渡之桥。但请记住，房子是租来的，而生活不是。
                                    </b>
                                </div>
                                <div>
                                    <b>
                                    </b>
                                </div>
                                <div>
                                    <br />
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row">
                <div class="cell">
                </div>
            </div>
            <!--/.row -->
        </div>
        <!-- /.container -->
    </footer>
    <div class="progress-wrap">
        <svg width="100%" height="100%" viewBox="-1 -1 102 102" class="progress-circle svg-content">
            <path d="M50,1 a49,49 0 0,1 0,98 a49,49 0 0,1 0,-98">
            </path>
        </svg>
    </div>
    <script src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/sandbox/assets/js/plugins.js"></script>
    <script src="https://template-1253409072.cos.ap-guangzhou.myqcloud.com/sandbox/assets/js/theme.js"></script>
    </div>
    </div>


    <footer class="white-section" id="footer">
        <div>
            <p style="font-size: small;margin: 40px;color: #8f8f8f;">
                数据来源及参考资料：<br>
                [1] 中华人民共和国教育部-教育统计数据
                http://www.moe.gov.cn/jyb_sjzl/moe_560/<br>
                [2] 中国联通智慧足迹《2021年全国大学生就业报告》<br>
                [3] 麦可思研究院《2022年中国大学生就业报告》<br>
                [4] 国家统计局- 70个大中城市商品住宅销售价格变动情况
                http://www.stats.gov.cn<br>
                [5] 禧泰数据-全国房价行情平台
                https://www.creprice.cn/<br>
                [6] ICCRA住房租赁产业研究院《2022年三季度中国住房租赁市场季度报告》<br>
                [7] 58安居客房产研究院《2022年毕业生租住报告》<br>
                [8] 豆瓣小组“我们在租房生活”
                https://www.douban.com/group/727449/<br>
                [9] 贝壳研究院《2022毕业季租住痛点调查报告》
                [10] 58安居客房产研究院《全国租赁市场11月报：40城超8成租金下跌 租赁供需持续走弱》
                https://mp.weixin.qq.com/s/JMtDn8n2OBFiG6FzSwEIuA<br>
                [11] 58安居客房产研究院《全国租赁市场10月报：市场价格平稳 供需进入淡季降幅10%左右》
                https://mp.weixin.qq.com/s/PopEvmUa07lnPfb75zYurA<br>
                [12] 58安居客房产研究院《2019年高校毕业生就业居行报告》<br>
                [13] 58安居客房产研究院《2020年毕业生居行调研报告》<br>
                [14] 58安居客房产研究院《2021年毕业生就业居住调研报告》<br>
                [15] 「长租视点」租得起与住得好 破局青年人的租房痛点
                https://baijiahao.baidu.com/s?id=1750181186805576837&wfr=spider&for=pc<br>
                [16] 后浪研究所-还没谈过恋爱的00后，开始和房子「相亲」了
                https://baijiahao.baidu.com/s?id=1736964951468846274&wfr=spider&for=pc<br>

            </p>
        </div>
        <div>
            <p style="text-align: center;color: #8f8f8f;font-size: small;">© Copyright2023 数据新闻第5组 吕翔新 谭相伶 刘雨辰 何雨馨 王竞翊
            </p>
        </div>

</body>

</html>
