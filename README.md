<!DOCTYPE html>
<html 朗="zh-CN">
<头>
    <元字符码="UTF-8">
    <标题>暖心提示弹窗</标题>
    <风格>
.提示窗口{
            位置: 已修复;
            填料: 20px;
            边界半径: 8px;
            框影: 0 4px 12px rgba(0, 0, 0, 0.15);
            字体系列: "微软雅黑", 无衬线;
            字体大小: 16px;
            颜色: #333;
z指数：9999；
            显示: 弯曲;
            对齐项目: 中心;
            证明内容: 中心;
            文本对齐: 中心;
        }
身体{
            利润: 0;
            填料: 0;
            背景色:#f8f9fa；
        }
    </风格>
</头>
<身体>
    <脚本>
        // 暖心提示语列表
        常量 小费 = [
            "多喝热水~", 保持微笑, "每天都要元气满满", 保持好心情, "好好爱自己",
            "梦想成真，顺顺利利", 早点休息, "愿所有烦恼都消失", "别熬夜", "注意保暖",
            "远离垃圾人垃圾事", 要微笑, "要开心", "要快乐", "要健康", "要平安", "要顺利",
            要幸福, "要好运"
        ];

        // 背景颜色列表
    常量bg颜色=【
    '浅粉色'，'天蓝色'，'浅绿色'，'薰衣草'，'淡黄色'，'乳白色'，
    '珊瑚'，'碧玺'，'海蓝宝石'，'蜜月玫瑰'，'蜂蜜露'，'桃酥'，
    '淡绿松石'，'薰衣草红'，'旧蕾丝'，'柠檬雪纺'，'浅蓝'，'淡灰'
        ];

        // 弹窗数量
    常量窗口数 = 550；
        // 弹窗生成间隔（毫秒）
    常数间隔 = 50；

        // 创建弹窗函数
    函数 createTipWindow（） {
    for （let i = 0; i < windowCount; i++） {
    设置超时时间={
    常量窗口 = document.createElement（'div'）；
    window.className = '提示窗口';
                    
                    // 随机选择提示语和背景颜色
    常量tip = tips[Math.floor（Math.random（） * tips.length）]；
    常量 bgColor = bgColors[Math.floor（Math.random（） * bgColor.length）]；
                    
                    // 设置弹窗样式
    window.style.backgroundColor = bgColor;
    window.style.width = `${250}px`;
    window.style.height = `${60}px`;
                    
                    // 随机设置弹窗位置
    常量屏幕宽度=窗口宽度。
    const screenHeight = window.innerHeight;
    常量x=随机数（）*（屏幕宽度—250）；
    常量y=随机数（）*（屏幕高度—60）；
    window.style.left = `${x}px'；
    window.style.top = `${y}px'；
                    
                    // 设置提示语内容
    提示；
                    
                    // 添加到页面
    文档。主体。附加子（窗口）；

                    // 弹窗显示一段时间后移除
    设置超时时间={
    文件.身体.删除孩子（窗口）；
                    }, 3000);
    }，i*间隔；
            }
        }

        // 页面加载完成后执行
    window.onload = createTipWindow;
    </script>
</身体>
</html>
