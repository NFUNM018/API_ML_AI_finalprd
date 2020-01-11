# API_ML_AI_finalprd
# 语法帮APP
### 展示ppt放在仓库里啦~需要麻烦评分的同学手动下载一下~~
如果下载出问题了麻烦微信dd我~我发给你~~
---

## 背景
当下社会科技正在飞速地进步，各种人工智能被越来越广泛地运用在我们生活中的不同领域。而当下教育行业也开始出现了各种智能设备的身影，它们帮助老师更好的进行传道授业解惑的教学，也帮助着学生更好的理解所要学习的知识。尤其是文科类的老师，常常要面对大量的文字作业，久了难免会疲于批改。那么是否有一款app能够自动识别文字作品中的错别字，尽可能地减少文字作品检查起来的难度呢？
## 加值宣言
通过百度**通用文字识别api**和AZURE**语音服务api**中的语音转文本功能帮助用户实现拍照或录音取字，调用百度**文本纠错api**帮助用户将语句录入后自动检查文章的错别字。尽可能减少用户在查找文章错别字时花费的时间与精力。还运用了AZURE的**文本翻译api**，帮助用户解决切换app复制翻译的过程。

# APP原型
- [APP原型在这里~](http://nfunm018.gitee.io/api_final)


- 原型核心功能展示
![图片1.png](https://upload-images.jianshu.io/upload_images/9467429-426cff775a83dffa.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片2.png](https://upload-images.jianshu.io/upload_images/9467429-b8a3f4e647989e9b.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片4.png](https://upload-images.jianshu.io/upload_images/9467429-701028211eeb282a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片5.png](https://upload-images.jianshu.io/upload_images/9467429-445fe1a219ce636c.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片6.png](https://upload-images.jianshu.io/upload_images/9467429-a140e698c77129bf.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片7.png](https://upload-images.jianshu.io/upload_images/9467429-0c7046a70e2ad24a.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片8.png](https://upload-images.jianshu.io/upload_images/9467429-7233f8129614e2fd.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)

![图片9.png](https://upload-images.jianshu.io/upload_images/9467429-36950457b11b4db4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)


## 目的
让老师不再花费太多精力，让学生更好地写出语句通顺的文章。
## 核心价值（最小可行性产品）

**文字识别**：完成将图片中的文字进行检测并转化录入进移动端中。

**基础语法纠错**：完成对文章中的字句用法进行检测，并将检查出的语法错误反馈给用户。
## 用户
- 需要花费大量精力批改学生文字作业的老师
- 文字组织能力还稍有欠缺的学生党
- 工作中需要写文件的文职人员、文字工作者
- 日常需要拍照取字翻译的用户
## 用户痛点
- 场景一：老师看着一大摞还未批改的作文发愁。
- 场景二：学生看着自己语句不通的文章发愁。
- 场景三：办公室职员一次次地检查自己文件的语法错误，生怕被老板扣工资。
- 场景四：看见一串外语（英、法、俄、西、葡、德、意、日、韩），想输入进手机后翻译，却发现自己没有相应的输入法导致无法录入。
## 人工智能概率性
- 文字识别出现错误：
有可能出现用户上传的图片有些许模糊，***识别图中文字时失败，或者识别错误***。
- 语法纠错：
有可能用户所上传的文章中使用了一些***歇后语、俚语、文言文***等非通俗语言，导致***语法纠错时无法识别。或者出现差错***。
## 需求列表与人工智能API加值
用户需求|所用API|重要程度
---|:--:|---:
拍照后将照片中的文字转化为文本|通用文字识别api|重要
查找文章中的语法错误|文本纠错api|重要
语句、词语翻译|文本翻译api|次重要



## API调用分析
api类别|所属平台|功能|优劣分析
---|:--:|---:|---:
文字识别|百度|对图片中的文字进行拍照检测|支持中、英、法、俄、西、葡、德、意、日、韩、中英混合等10种语言识别，同时支持中、英、日、韩四语种的类型检测
文字识别|阿里|对图片中的文字进行拍照检测|可用于识别合同、文档、小说等图片，用于合同校对、文档检索、pdf提取等场景

可以看到，虽然百度与阿里均有通用文字识别api服务，但是阿里的文字识别api功能百度也均可以达到。并且百度的文字识别api还支持中、英、法、俄、西、葡、德、意、日、韩、中英混合等10种语言识别，这一点便比阿里的更有优势。

- 价格对比
![定价.png](https://upload-images.jianshu.io/upload_images/9467429-7145860bd64d97b4.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
百度的定价

![定价2.png](https://upload-images.jianshu.io/upload_images/9467429-9acff30093cc903d.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
阿里的定价

可以看出百度的定价与阿里相比还是更加便宜实惠的。因此最终还是选择百度的文字检测api。



## 具体应用场景：
- 场景一：工作了一天回到家的语文老师还有一摞学生的阅读理解要批改。忙完自己的事已经已经夜深，老师打开了app，将学生的文章拍照录入，并将其都录入进手机里。第二天上班的地铁上，老师打开了手机中昨晚录入的学生作业一一查看，并及时记录下了同学们出错最多的题目。
- 场景二：小明在看书的时候，在书中出现了一句葡萄牙语，小明很想知道这句话是什么意思，他掏出手机却发现自己不会打葡萄牙语。他邪魅一笑，打开了“语法帮app”，选中了拍照功能，将那句葡萄牙语拍了下来，瞬间手机屏幕上就出现了那句话，他点击句子后出现的“翻译”按钮，成功将葡萄牙语翻译成了中文。
- 场景三：小明工作时需要写大量的文档，他又有一些粗心马虎，常常出现因文档中的语法错误而被扣工资的现象。那天，他打开了语法帮app，将写好的文档上传，app自动为他检测出了文档中的语法错误。

API代码：
- 图片文字识别：

```

from aip import AipOcr
import os



APP_ID = '17993129'
API_KEY = 'lMedlFKXqiyHgtnQDjY94Mpz'
SECRET_KEY = 'xxxxxxxxxxx'

client = AipOcr(APP_ID, API_KEY, SECRET_KEY)


def get_file_content(filePath):
    with open(filePath, 'rb') as fp:
        return fp.read()

PROJECT_ROOT = os.path.dirname(os.path.realpath(__file__))
path = os.path.join(PROJECT_ROOT,"‪D:\test\image.jpg")
for r, ds, fs in os.walk(path):
     for fn in fs:
        fname = os.path.join(r, fn)
        image = get_file_content(fname)
        ret = client.basicGeneral(image)
        for item in ret['words_result']:
            print(item['words'])
```
- 识别结果返回：
```
{
	"log_id": "8581649843797602188",
	"words_result_num": 2,
	"words_result": [
		{
			"words": "计算机应用基础实验教程"
		},
		{
			"words": "军事理论与军事技能"
		}
	]
}
```

