encoding: utf-8
@email: 1253039341@qq.com
@time: 2020/8/13 11:36

__author__ = "山东少年先锋队"
__version__ = "0.0.1"


相比于原始HTMLTestRunner
增加：
* 支持中文，汉化
* 调整样式，美化（需要连入网络，使用的cdn的Bootstrap.js）
* 增加 可根据用例名称和结果搜索
* 增加 扇形图，用来展示成功率
* 优化“展开”与“收缩”状态的变换
* 美化汇总报告
* 美化详细数据


感谢各位开源作者的无私奉献，参考学习链接：

HTMLTestRunner： http://tungwaiyip.info/software/HTMLTestRunner.html

Joy_QA_Platform：https://github.com/JoyMobileDevelopmentTeam/Joy_QA_Platform

肯定存在bug，可以的话请告诉我，之后有需要会再出一版修复bug，希望对大家有帮助

使用方法例：

    import HTMLTestRunner2020
    
    ..................
    
    suite = "你的用例"
    
    runner = HTMLTestRunner2020.HTMLTestRunner("报告输出位置", verbosity=2, title="自动化测试标题",)
    
    try:
    
        runner.run(suite)
        
        except Exception as e:
        
        MyLogs().error("执行用例失败:{0}".format(e))
        
生成的测试报告样例：

https://github.com/yinhuajun/HTMLTestRunner2020/blob/master/report.html

样例效果：

![Image text](https://github.com/yinhuajun/HTMLTestRunner2020/blob/master/20200818142002.png)
