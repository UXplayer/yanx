
![img.png](docs/img/img.png)

**YanX 是一个一键下载全国所有院校*硕士研究生专业目录*的工具**

**更便捷更快速的将全部院校做对比和分析，基于考试科目，招生人数，院校建设划，院校地区，寻找最棒最合适的院校！**


## 快速使用

### 1. 下载

1. *学位类别*：先选择 *学术学位* 或 *专业学位* 中的一个；

2. *门类类别*：如果学位类别选择了专业学位则门类类别中只有*专业学位*可选；如果选择了学术学位，则会有多个门类可选；


3. *学科类别*：对应不同的门类有不同的学科类别，选择一个学科类别，就可以开始下载了。

此外还有一些可选择项目

1. *专业名称* ：部分学科对应多个专业，有其他的专业名称，则可以选择其中的一个

2. *学习方式* ：学习方式可选择全日制、非全日制

3. *院校建设计划*：部分学校属于985、211或双一流院校，可以选择其中的一项，或者排除重点院校只选择普通院校

4. *院校区域* ：此区域非省份地区，而是指考研院校中的A类考试和B类考生省份区域

### 2. 导出

下载完成后的任务可以进行导出，对多个下载任务可以导出到同一个文件、也可以每一个任务导出到单独的文件；例如可以将 学硕-0821 和
专硕-0854 导出到同一个文件中。

下图是选择 [学术学位-0201理论经济学-全日制](https://github.com/xx025/YanX/blob/pages/docs/%E5%AD%A6%E6%9C%AF%E5%AD%A6%E4%BD%8D-0201%E7%90%86%E8%AE%BA%E7%BB%8F%E6%B5%8E%E5%AD%A6-%E5%85%A8%E6%97%A5%E5%88%B6-2022-09-16-8.csv)
的导出文件内容

![202304141631960](https://st.ai55.cc/img/202304141631960.png)

### 3. Excel 筛选

通过表格软件Excel或WPS打开导出的文件，你可以选择第一行用表格软件的筛选工具，进行更进一步的筛选

比如 具体的考试科目，比如外语一般分为 英语（一）和英语（二），或具体专业课，或选中排除个别省份地区，筛选掉招生人数较少的院校等，等等各种筛选不再一一赘述。

## 资料参考

[AB类地区和985、211院校目录](docs/AB类地区和985、211院校目录)

[院校库.csv](docs/院校库.csv)
，数据来自于研招网[院校库](https://yz.chsi.com.cn/sch/)

## 调试与开发

当前项目有两个库，一个是当前库，它用 FastAPI 用做前端界面，另一个是 [yzw-dl](https://github.com/xx025/yzw-dl) 它是下载研招网数据的核心库

```shell
git clone -b main https://github.com/xx025/yanx.git yanx
cd yanx
conda create -n yanx python=3.8 -y;conda activate yanx # 使用 conda 创建虚拟环境
pip install -r requirements.txt
python run.py
```

## 声明

1. 本软件只供学习交流使用，勿作为商业用途
2. 对使用本软件造成的任何影响，概不负责


