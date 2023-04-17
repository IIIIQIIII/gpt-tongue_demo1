# gpt-tongue_demo1

## content

1.1 介绍
中医舌诊AI开放平台
中医舌诊AI开放平台隶属于合肥云诊信息科技有限公司。中医在几千年的实践过程中，总结了相对完整的舌诊临床意义，随着舌诊技术的发展，很多疾病与舌象特征的变化规律还需要进一步挖掘与研究。
安徽中医药大学与合肥云诊信息科技有限公司联合研发了“中医舌诊AI开放平台”，平台以海量的舌象大数据为基础，结合机器学习、深度学习的神经网络算法，对舌象特征进行精准的检测与识别、多维度的定量化分析，为中医院、中医高校、科研机构提供舌象与病种关系的研究，为大众提供中医健康状态辨识服务。

2.2 术语表
术语表
中医体质
《中医体质分类与判定》标准的九个类型体质及其组合的兼夹体质。

健康状态
中医健康状态是人生命过程中受到自然、社会等因素变化的刺激、人体脏腑、经络、气血作出与之相适应的调整而形成的生命态。
涵盖了中医体质及脏腑病位（心、肝、脾、肺、肾）、病性（气虚、血瘀、痰、寒等）的辨证构成的中医证名。

2.3 数据枚举
数据枚举
性别
值	描述
0	未知
1	男性
2	女性
舌象特征（6.1.舌象特征API）
特征项	值
舌色	淡白舌、舌质淡、淡红舌、红舌、绛舌、青紫舌
苔色	白苔、淡黄苔、黄苔、焦黄苔、灰黑苔、焦黑苔
苔质	薄苔、厚苔、腐、腻、剥落、无苔、少苔
舌形	胖、瘦、老、嫩、点刺、瘀斑、瘀点、裂纹、齿痕
津液	润、滑、燥
舌下络脉	舌下正常、舌下虚象、舌下瘀象、舌下图不清晰
中医体质（6.2.体质辨识API）
单一体质
编码	值
1	平和
2	气郁
3	气虚
4	血虚
5	阳虚
6	阴虚
7	痰湿
8	湿热
9	实热
10	血瘀
11	特禀
兼夹体质
编码	值	单一构成编码	单一构成名称
21	气血两虚	3,4	气虚,血虚
22	气阴两虚	3,6	气虚,阴虚
23	气虚血瘀	3,10	气虚,血瘀
24	阳虚血瘀	5,10	阳虚,血瘀
25	血虚血瘀	4,10	血虚,血瘀
26	阴虚血瘀	6,10	阴虚,血瘀
27	痰瘀互结	10,7	血瘀,痰湿
28	湿热血瘀	8,10	湿热,血瘀
29	瘀热互结	9,10	实热,血瘀
30	气滞血瘀	2,10	气郁,血瘀
31	气滞湿阻	2,7	气郁,痰湿
32	气滞湿热	2,8	气郁,湿热
33	气虚痰湿	3,7	气虚,痰湿
34	阳虚痰湿	5,7	阳虚,痰湿
35	阴虚痰湿	6,7	阴虚,痰湿
36	阴虚湿热	6,8	阴虚,湿热
37	气虚湿热	3,8	气虚,湿热
38	阴虚阳亢	6,9	阴虚,实热
71	气血两虚夹瘀	3,4,10	气虚,血虚,血瘀
72	气阴两虚夹瘀	3,6,10	气虚,阴虚,血瘀
73	气滞湿阻夹瘀	2,7,10	气郁,痰湿,血瘀
74	气滞湿热夹瘀	2,8,10	气郁,湿热,血瘀
75	气虚痰湿夹瘀	3,7,10	气虚,痰湿,血瘀
76	阳虚痰湿夹瘀	5,7,10	阳虚,痰湿,血瘀
77	阴虚痰湿夹瘀	6,7,10	阴虚,痰湿,血瘀
78	阴虚湿热夹瘀	6,8,10	阴虚,湿热,血瘀
79	气虚湿热夹瘀	3,8,10	气虚,湿热,血瘀
80	阴虚阳亢夹瘀	6,9,10	阴虚,实热,血瘀
健康状态（6.3.中医辨识API）
编码	值	证型
1	平和	-
2	气郁	肝郁气滞证、胃肠气滞证、肝郁脾虚证、肝胃不和证
3	气虚	心气虚证、肺气虚证、肾气虚证、脾气虚证、胃气虚证、心脾气虚证、
心肾气虚证、心肺气虚证、肺胃气虚证、肺脾气虚证、肺肾气虚证、脾胃气虚证、
脾肾气虚证
4	血虚	心血虚证、肝血虚证、心肝血虚证
5	阳虚	心阳虚证、脾阳虚证、肾阳虚证、胃阳虚证、虚水泛证、心脾阳虚证、
心肾阳虚证、脾肾阳虚证、脾胃阳虚证
6	阴虚	心阴虚证、肝阴虚证、肺阴虚证、肾阴虚证、胃阴虚证、肠燥津亏证、
肝阳上亢证、心肺阴虚证、心肾不交证、肺肾阴虚证、肺胃阴虚证、肺肝阴虚证、
肝肾阴虚证
7	痰湿	痰蒙心神证、寒湿困脾证、饮停胸胁证、痰阻心脉证、痰浊阻肺证、食积胃肠证
8	湿热	大肠湿热证、湿热蕴脾证、膀胱湿热证、肝胆湿热证、痰热壅肺证、胆郁痰扰证
9	实热	心火亢盛证、肺热炽盛证、胃热炽盛证、肝火炽盛证、肝火犯肺证、小肠实热证
10	血瘀	瘀阻心脉证、瘀阻脑络证、胃脘瘀阻证、瘀阻胞宫证、肝脉瘀阻证
11	特禀	-
21	气血两虚	-
22	气阴两虚	-
23	气虚血瘀	-
24	阳虚血瘀	-
25	血虚血瘀	-
26	阴虚血瘀	-
27	痰瘀互结	-
28	湿热血瘀	-
29	瘀热互结	-
30	气滞血瘀	-
31	气滞湿阻	-
32	气滞湿热	-
33	气虚痰湿	-
34	阳虚痰湿	-
35	阴虚痰湿	-
36	阴虚湿热	-
37	气虚湿热	-
38	阴虚阳亢	-
71	气血两虚夹瘀	-
72	气阴两虚夹瘀	-
73	气滞湿阻夹瘀	-
74	气滞湿热夹瘀	-
75	气虚痰湿夹瘀	-
76	阳虚痰湿夹瘀	-
77	阴虚痰湿夹瘀	-
78	阴虚湿热夹瘀	-
79	气虚湿热夹瘀	-
80	阴虚阳亢夹瘀	-
检测类别
体质与健康状态（C00）
编码	名称
C00.D00	体质与健康状态
“6.2. 体质辨识API”结果参考这里
“6.3. 中医辨识API”结果参考这里
女性疾病（C01）
编码	名称
C01-C00-C00.D00	月经先期
C01-C00-C00.D01	月经后期
C01-C00-C00.D02	月经先后无定期
C01-C00-C00.D03	经期延长
C01-C00-C00.D04	经间期出血
C01-C00-C01.D00	月经过多
C01-C00-C01.D01	月经过少
C01-C00-C02.D00	崩漏
C01-C00-C02.D01	闭经
C01-C00-C03.D00	痛经
C01-C00-C03.D01	经行乳房胀痛
C01-C00-C03.D02	经行头痛
C01-C00-C04.D00	经行发热
C01-C00-C04.D01	经行眩晕
C01-C00-C04.D02	经行浮肿
C01-C00-C04.D03	经行泄泻
C01-C00-C04.D04	经行情志异常
C01-C00-C05.D00	更年期综合征
C01-C00-C05.D01	绝经后出血
C01-C01.D00	带下过多
C01-C01.D01	带下过少
C01-C02.D00	产后腹痛
C01-C02.D01	产后身痛
C01-C02.D02	产后发热
C01-C02.D03	产后自汗、盗汗
C01-C02.D04	产后大便难
C01-C02.D05	产后小便淋痛
C01-C02.D06	产后情志异常
C01-C03.D00	不孕症
C01-C03.D01	多囊卵巢综合症
C01-C03.D02	子宫内膜异位症
C01-C03.D03	慢性盆腔炎
C01-C03.D04	妇人腹痛（腹内没有包块）
C01-C03.D05	妇人腹痛（腹内有包块）
儿童调理（C02）
编码	名称
C02.D00	儿童体质辨识
慢病调理（C04）
编码	名称
C04.D00	高血压
C04.D01	冠心病
C04.D02	糖尿病
儿童常见疾病（C08）
编码	名称
C08.D00	脾胃病
C08.D01	咳嗽
C08.D02	感冒
C08.D03	哮喘
面部特征
特征项	值
面色	面色红黄隐隐，明润含蓄、面色晦暗枯槁或暴露浮现
主色	正常、面赤、面黄、面白、面黑、面青
光泽	正常、少量、无
黑眼圈	正常、轻度、重度、不符合要求（装扮或眼部受伤）
唇色	正常、白 、红、暗红、青紫 、黑色或斑点、不符合检测要求
眼神	有神、少神、不符合检测要求
目色	正常、目赤肿胀、目黄、不符合检测要求
两颧红	正常、轻度
鼻褶	无 、轻度、重度
眉间/鼻柱青色	正常、眉间有青色
面部皮损	正常、疑似色素痣、皮下颗粒物、疑似皮肤病，需进一步检测
耳色	正常、白、红、黄、青紫、不符合检测要求
耳褶	无、轻度、重度、不符合检测要求

2.4 错误码
<table>
<thead>
<tr>
<th>错误码(code)</th>
<th>错误描述(msg)</th>
<th>问题排查策略</th>
</tr>
</thead>
<tbody>
<tr>
<td>1002001</td>
<td>http请求方法不支持</td>
<td>-</td>
</tr>
<tr>
<td>1008997</td>
<td>参数异常</td>
<td>-</td>
</tr>
<tr>
<td>1009999</td>
<td>系统内部错误，请联系管理员</td>
<td>云诊平台内部错误，请联系云诊管理员</td>
</tr>
<tr>
<td>1200006</td>
<td>非可信任客户端程序</td>
<td>对接应用 ID 或应用密钥错误</td>
</tr>
<tr>
<td>1200007</td>
<td>用户不存在</td>
<td>点数充值对象用户不存在</td>
</tr>
<tr>
<td>1200009</td>
<td>应用已被禁用</td>
<td>检查企业是否被禁用并联系云诊管理员</td>
</tr>
<tr>
<td>1200024</td>
<td>此应用不支持单点登录</td>
<td>-</td>
</tr>
<tr>
<td>1200025</td>
<td>单点登录验签不通过</td>
<td>接口传参签名错误</td>
</tr>
<tr>
<td>1200033</td>
<td>应用不存在</td>
<td>请确认H5接入应用参数</td>
</tr>
<tr>
<td>2500001</td>
<td>企业不存在</td>
<td>请联系云诊管理员确认企业信息</td>
</tr>
<tr>
<td>2500003</td>
<td>接口不存在</td>
<td>-</td>
</tr>
<tr>
<td>2500005</td>
<td>计费规则不存在</td>
<td>API应用接口未配置计费规则，请联系云诊管理员</td>
</tr>
<tr>
<td>2500007</td>
<td>企业账户余额不足</td>
<td>企业账户点数不足或API应用接口可用时长已到</td>
</tr>
<tr>
<td>2500020</td>
<td>企业账户点数不足</td>
<td>使用点数充值功能进行充值</td>
</tr>
</tbody>
</table>
<h2 id="h5应用开放对接"><a name="h5应用开放对接" class="plugin-anchor" href="http://www.ai-tongue.com/doc/global/errorCode.html#h5%E5%BA%94%E7%94%A8%E5%BC%80%E6%94%BE%E5%AF%B9%E6%8E%A5"><i class="fa fa-link" aria-hidden="true"></i></a>H5应用开放对接</h2>
<table>
<thead>
<tr>
<th>错误码(code)</th>
<th>错误描述(msg)</th>
<th>问题排查策略</th>
</tr>
</thead>
<tbody>
<tr>
<td>2410001</td>
<td>参数获取失败</td>
<td>-</td>
</tr>
<tr>
<td>2410005</td>
<td>充值点数超出剩余点数</td>
<td>使用点数充值功能进行充值</td>
</tr>
<tr>
<td>2410100</td>
<td>确认检测点数大于0</td>
<td>-</td>
</tr>
<tr>
<td>2410102</td>
<td>解密错误，请确认平台rsa公钥（rsaPublicKey）正确</td>
<td>接口传参加密出错</td>
</tr>
<tr>
<td>2410104</td>
<td>验签错误，请确认开发者rsa私钥（devRsaPrivateKey）正确</td>
<td>接口传参签名出错</td>
</tr>
<tr>
<td>2410105</td>
<td>签名为空</td>
<td>接口参数<code>signEncryptedJson</code>为必填项</td>
</tr>
<tr>
<td>2410106</td>
<td>加密数据为空</td>
<td>接口传参无加密数据</td>
</tr>
<tr>
<td>2410107</td>
<td>解密数据json解析出错</td>
<td>接口传参解密后格式不是JSON</td>
</tr>
<tr>
<td>2410108</td>
<td>不支持会员接口充值</td>
<td>H5接入应用不支持会员接口充值</td>
</tr>
</tbody>
</table>
<h2 id="api接口开放对接"><a name="api接口开放对接" class="plugin-anchor" href="http://www.ai-tongue.com/doc/global/errorCode.html#api%E6%8E%A5%E5%8F%A3%E5%BC%80%E6%94%BE%E5%AF%B9%E6%8E%A5"><i class="fa fa-link" aria-hidden="true"></i></a>API接口开放对接</h2>
<table>
<thead>
<tr>
<th>错误码(code)</th>
<th>错误描述(msg)</th>
<th>问题排查策略</th>
</tr>
</thead>
<tbody>
<tr>
<td>2609001</td>
<td>第三方单据唯一标识为空</td>
<td>接口参数<code>outId</code>为必填项</td>
</tr>
<tr>
<td>2609002</td>
<td>第三方单据唯一标识已存在</td>
<td>接口参数<code>outId</code>重复</td>
</tr>
<tr>
<td>2609003</td>
<td>文件不存在</td>
<td>接口参数<code>images</code>为必填项</td>
</tr>
<tr>
<td>2609004</td>
<td>上传文件到OSS失败</td>
<td>-</td>
</tr>
<tr>
<td>2609015</td>
<td>解密错误，请确认aeskey正确</td>
<td>接口传参解密出错</td>
</tr>
<tr>
<td>2609017</td>
<td>验签错误，请确认开发者rsa私钥（devRsaPrivateKey）正确</td>
<td>接口传参签名出错</td>
</tr>
<tr>
<td>2609018</td>
<td>签名为空</td>
<td>接口参数<code>signature</code>为必填项</td>
</tr>
<tr>
<td>2609019</td>
<td>加密数据为空</td>
<td>接口参数<code>encryptData</code>为必填项</td>
</tr>
<tr>
<td>2609020</td>
<td>解密数据json解析出错</td>
<td>接口传参解密后格式不是JSON</td>
</tr>
<tr>
<td>2609021</td>
<td>分析任务不存在</td>
<td>-</td>
</tr>
<tr>
<td>2609022</td>
<td>预分析任务不存在</td>
<td>-</td>
</tr>
<tr>
<td>2609023</td>
<td>问诊回答对应问诊不存在或已经处理</td>
<td>-</td>
</tr>
<tr>
<td>2609027</td>
<td>预分析任务尚未完成</td>
<td>请等待预分析任务完成</td>
</tr>
<tr>
<td>2609028</td>
<td>预分析任务不是成功状态</td>
<td>-</td>
</tr>
</tbody>
</table>
<h2 id="api接口回调"><a name="api接口回调" class="plugin-anchor" href="http://www.ai-tongue.com/doc/global/errorCode.html#api%E6%8E%A5%E5%8F%A3%E5%9B%9E%E8%B0%83"><i class="fa fa-link" aria-hidden="true"></i></a>API接口回调</h2>
<table>
<thead>
<tr>
<th>错误码(code)</th>
<th>错误描述(msg)</th>
<th>问题排查策略</th>
</tr>
</thead>
<tbody>
<tr>
<td>-1</td>
<td>未知错误</td>
<td>请反馈给系统管理员</td>
</tr>
<tr>
<td>201</td>
<td>图片过暗</td>
<td>需要使用清晰的舌象图片</td>
</tr>
<tr>
<td>202</td>
<td>图片过亮</td>
<td>需要使用清晰的舌象图片</td>
</tr>
<tr>
<td>203</td>
<td>图片不是舌头（请拍摄带有舌头的、清晰的彩色照！）</td>
<td>-</td>
</tr>
<tr>
<td>204</td>
<td>未提取到舌头（照片带有舌头，只是模型不完善，导致提取不到）</td>
<td>-</td>
</tr>
<tr>
<td>205</td>
<td>系统内部错误</td>
<td>需要使用清晰的舌象图片；常见原因是图片过小300KB以下</td>
</tr>
<tr>
<td>206</td>
<td>图片不是舌下（请拍摄带有舌下的、清晰的彩色照！）</td>
<td>-</td>
</tr>
<tr>
<td>300</td>
<td>未分析出健康状态</td>
<td>先尝试使用清晰的舌象图片，如果还是提示错误，则反馈给系统管理员</td>
</tr>
</tbody>
</table>

2.5 常见问题
常见问题
注册登录
详见 注册登录-常见问题

微信应用开放对接
详见 微信应用开放对接-常见问题

H5应用开放对接
详见 H5应用开放对接-常见问题

舌象特征API
详见 舌象特征API-常见问题

面象特征API
详见 面象特征API-常见问题

体质辨识API
详见 体质辨识API-常见问题

中医辨识API
详见 中医辨识API-常见问题

接入流程

3.1 注册登录
注册
注册流程
1、进入 中医舌诊AI开放平台，单击页面右上角 登录 按钮，选择 企业登录，进入 AI 舌诊对接 登录页面，点击页面下方 没有账号？点此注册。

2、填写注册信息，阅读服务条款，单击 我已阅读并同意服务协议和法律声明及隐私权政策。

输入企业名称；
输入登录名：
只能使用大小写字母和数字。
尽量避免使用姓名、手机号、身份证、银行卡等隐私信息。
输入密码：
只能使用大小写字母和数字。
尽量避免使用姓名、手机号、身份证、银行卡等隐私信息。
输入确认密码；
输入手机号：
请使用中国大陆的手机号。
3、获取短信验证码，输入您的手机收到的验证码；

4、点击注册按钮，提示注册成功。

常见问题
登录名已存在：请修改登录名重新注册。
手机号已被使用：
更换手机号重新注册。
可以使用该手机号继续完成注册（注册新企业），但是输入的登录名和密码不会创建新账号，而自动绑定已存在账号的登录名和密码。
如果该手机号被使用的账号不为您所有，请联系客服400-888-7378。
登录
登录流程
进入 中医舌诊AI开放平台，单击页面右上角 登录 按钮，选择 企业登录。可选择 微信扫码登录 和 账号密码登录。

微信扫码登录
打开微信扫一扫页面显示的二维码，在手机上同意微信授权。会出现以下情况：

弹框提示用户不存在：请先注册账号；
该账号下只存在一个企业用户，直接登录成功，进入后台；
该账号下存在多个企业用户，选择一个企业用户，登录成功后进入后台。
账号密码登录
填写用户名、密码进行登录。会出现以下情况：

账号或者密码错误：请检查您输入的账号和密码是否正确；
该账号下只存在一个企业用户，直接登录成功，进入后台；
该账号下存在多个企业用户，选择一个企业用户，登录成功后进入后台。

3.2 企业认证
企业认证
刚注册的企业需要进行企业认证，登录成功后会自动弹出 尚未进行企业认证，无法创建应用及调用API。 是否前往认证 弹框，点击确认按钮后前往企业认证页面。

填写企业基本信息
填写企业基本信息，主要包括如下字段：

证照类型：选择需要上传的组织证照类型：
营业执照；
非营业执照：非营业执照指的是各类企业登记证书、许可证书、企业执照、三证合一类证书等非营业执照类型的企业组织证照。
组织证照：上传营业执照或者非营业执照的截图，大小不超过 5 M。
医疗机构执业资格许可证：上传医疗机构执业资格许可证的截图，大小不超过 5 M。
企业名称；
机构代码：机构代码是对中华人民共和国内依法注册、依法登记的机关、企事业单位、社会团体，以及其他组织机构颁发一个在全国范围内唯一的、始终不变的代码标识。请填入证照上的统一社会信用代码或注册号或组织机构代码。
通讯地址：请选择企业所在的省市区；
详细地址：请填写企业的详细地址；
公司官网；
对接等级表：请先下载《对接登记表》模板，填写后盖公司章，扫描做成pdf文件上传。
认证信息审核
提交企业基本信息，等待平台审核；如果审核不通过，会显示不通过原因，可以返回修改然后再提交审核。

认证完成
如果平台审核通过，则表示企业已认证通过。

授权接口

4.1 获取access_token
获取access_token
接口描述
第三方用户可通过调用开放平台提供的API获取舌象特征、进行体质辨识以及健康状态辨识，因为涉及数据隐私，所以在使用前必须获得授权。

接入流程
注册为开放平台用户；
提交企业信息认证，等待平台审核通过；
新建API应用或H5应用，获取应用devid和devsecret；
通过验证授权接口，获取access_token；
使用access_token进行后续接口调用。
获取access_token接口
请求地址
https://www.ai-tongue.com/backend/auth/invoker/pwd/signin

请求方法
POST

传参形式
form-data

请求示例
Postman导出的请求示例如下，您也可以导入Postman后查看
{
 "info": {
     "_postman_id": "30ed5c93-452f-4759-b830-b19f8b8d9f02",
     "name": "Demo_获取access_token",
     "schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
 },
 "item": [
     {
         "name": "获取access_token",
         "request": {
             "auth": {
                 "type": "noauth"
             },
             "method": "POST",
             "header": [],
             "body": {
                 "mode": "formdata",
                 "formdata": [
                     {
                         "key": "devid",
                         "value": "your_devid",
                         "type": "text"
                     },
                     {
                         "key": "devsecret",
                         "value": "your_devsecret",
                         "type": "text"
                     }
                 ]
             },
             "url": {
                 "raw": "https://ai-tongue.com/backend/auth/invoker/pwd/signin",
                 "protocol": "https",
                 "host": [
                     "ai-tongue",
                     "com"
                 ],
                 "path": [
                     "backend",
                     "auth",
                     "invoker",
                     "pwd",
                     "signin"
                 ]
             }
         },
         "response": []
     }
 ]
}
请求参数
参数	格式	是否必须	含义
devid	String	必须	应用ID
devsecret	String	必须	应用密钥
响应示例
{
    "code": 0,
    "msg": "成功",
    "data": {
        "access_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2MTY1NzMxMzYsInVzZXJfbmFtZSI6InRlc3RBcHAiLCJqdGkiOiIzYWJjOTFlNy0yNGRlLTRlYzYtYjMzOS1kYzM1ODA3NDUwMjkiLCJjbGllbnRfaWQiOiJ0ZXN0QXBwIiwic2NvcGUiOlsiKiJdfQ.WIGQU2QglKm4iytJUmxjyq9rM7l86SOzW4rTqgpv1mg",
        "token_type": "bearer",
        "refresh_token": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2MTY1NzMxMzYsInVzZXJfbmFtZSI6InRlc3RBcHAiLCJqdGkiOiI0MzI1NzVkMy0yMzQ3LTQxNTUtODNkZS1lNjhmNzI3Yjg5MWQiLCJjbGllbnRfaWQiOiJ0ZXN0QXBwIiwic2NvcGUiOlsiKiJdLCJhdGkiOiIzYWJjOTFlNy0yNGRlLTRlYzYtYjMzOS1kYzM1ODA3NDUwMjkifQ.Un7PgSYMjWhV_0Ju6V9P2GX7rymnXYOAXNij4FgCld4",
        "expires_in": 1799,
        "scope": "*",
        "jti": "3abc91e7-24de-4ec6-b339-dc3580745029"
    }
}
响应参数
参数	格式	描述
code	Number	0成功，其他为失败
msg	String	响应结果描述
data	Object	响应数据
data.access_token	String	授权访问token
data.token_type	String	目前为bearer
data.refresh_token	String	刷新token
data.expires_in	Number	token有效期，单位为秒
data.scope	String	用户登陆的作用域范围，目前为*
错误码说明
错误码详细信息请参见：错误码

access_token的使用
在需要鉴权的接口调用时，HTTP请求头中添加:

Authorization ：Bearer access_token

页面快速集成方式

5.2. H5应用开放对接
H5应用开放对接
对接介绍
开发者可以将AI舌诊移动H5端完整功能集成到目标app中。用户使用开发者app，通过菜单进入AI舌诊系统完成舌诊体验。

5.2.2. 单点登录接口
单点登录接口
接口调用请求说明
请求地址 https://www.ai-tongue.com/h5/sso

请求方法 GET

请求示例
GET https://www.ai-tongue.com/h5/sso?access_token=123456&encryptedThirdId=123456
&signEncryptedThirdId=123456&capture=all&diseaseCode=C00.D00
请求参数
名称	格式	是否必须	含义
access_token	String	是	通过getAccessToken获取
encryptedThirdId	String	是	使用平台公钥(rsaPublicKey)
对第三方用户唯一标识进行RSA加密后的字符串
signEncryptedThirdId	String	是	使用应用私钥(devRsaPrivateKey)
对encryptedThirdId进行RSA签名后的字符串
userName	String	否	用户姓名
sex	String	否	用户性别：0未知 1男 2女
birthday	String	否	出生日期，日期格式： yyyy-MM-dd
capture	String	否	默认：选择舌象时支持文件资源和相机拍照
all：选择舌象时支持文件资源和相机拍照
camera：选择舌象时仅支持相机拍照
diseaseCode	String	否	检测类别编码，默认值为C00.D00（体质与健康状态）
中医慢病、妇科病和儿童常见病的检测类别编码请参考 检测类别
登录成功
引导完善信息：验证用户是否是第一次登录，验证用户是否存在于舌诊平台
用户第一次登录或不存在于舌诊平台则导航到用户注册完善信息页面
引导用户完成手机号、姓名、年龄基本信息完善
直接登录：直接跳转到AI健康云诊首页

5.2.3. 点数充值接口
点数充值接口
接口调用请求说明
请求地址 https://www.ai-tongue.com/backend/check/i/secret/point/recharge

请求方法 POST

请求示例
POST https://www.ai-tongue.com/backend/check/i/secret/point/recharge

请求头： Authorization ：Bearer access_token（通过getAccessToken获取）

请求参数

{
    "encryptedJson": "encryptedJson",
    "signEncryptedJson": "signEncryptedJson"
}
请求参数
名称	格式	是否必须	含义
encryptedJson	String	是	使用平台公钥(rsaPublicKey)
对原文进行RSA加密后的字符串
signEncryptedJson	String	是	使用应用私钥(devRsaPrivateKey)
对encryptedJson进行RSA签名后的字符串
原文实例
{
    "checkPoint": 10,
    "thirdId": "thirdId"
}
原文参数
名称	格式	是否必须	含义
checkPoint	Number	是	充值的点数数量
thirdId	String	是	用户第三方Id，即集成方用户ID
响应示例
成功

{
  "code": 0,
  "msg": "成功"
}
失败

{
  "code": 1200007,
  "msg": "充值用户不存在"
}
响应参数
名称	格式	含义
code	Number	0成功，其他为失败
msg	String	响应结果描述
错误码说明
错误码详细信息请参见：错误码

5.2.4. 支付回调
支付回调
接口描述
用于舌诊平台回传用户使用点数支付成功的通知

参数名称和字段类型固定
接收到支付通知，先验证签名，再解密通知数据
舌诊平台最多尝试3次回调通知，均无响应则不再通知。
充值、支付操作，可通过AI开放平台系统进行对账查询（系统开发中）。
接口说明
请求地址 系统集成方提供的支付成功后通知地址

请求方法 POST

请求参数
名称	格式	是否必须	含义
encryptedJson	String	是	使用应用公钥(devrsaPublicKey) 对原文进行RSA加密后的字符串
signEncryptedJson	String	是	使用平台私钥(rsaPrivateKey) 对encryptedJson进行RSA签名后的字符串。 建议开发者接收到请求后对signEncryptedJson 验证签名以保证系统安全性。
原文实例
{
    "recordId": "0",
    "returnType": 1,
    "thirdId": "thirdId"
}
原文参数
名称	格式	是否必须	含义
recordId	String	是	舌诊报告记录唯一标识
returnType	Number	是	固定值1，表示用户个人点数方式支付
thirdId	String	是	用户第三方Id，即集成方用户ID

5.2.5 实例代码
目前Android、iOS版提供完整集成使用示例。

Android版例子
https://gitee.com/ai-tongue/ai-tongue-h5-android

iOS版例子
https://gitee.com/ai-tongue/ai-tongue-h5-ios

5.2.6. 常见问题
常见问题
调用接口时，系统返回 “验签错误，请确认开发者rsa私钥（devRsaPrivateKey）正确”
先检查是不是使用开发参数中的devRsaPrivateKey字段进行签名操作的。
再检查是不是使用的是示例代码中的RSA工具类。
调用接口时，系统返回 “解密错误，请确认平台rsa公钥（rsaPublicKey）正确”
先检查是不是使用开发参数中的rsaPublicKey字段进行加密操作的。
再检查是不是使用的是示例代码中的RSA工具类。
Android版问题
1、中医AI舌诊页面点击上传舌象图片不能打开相册或相机。
image

问题原因：webview不能让h5自己调用相册或相机。

解决方法：自行实现调用相册和相机。

2、健康状态报告页面使用微信支付，提示错误“商家参数格式错误，请联系商家解决”。
image

问题原因与解决方法：
如果是APP里调起H5支付，需要在WebView中手动设置Referer，如：

Map extraHeaders = new HashMap();
extraHeaders.put("Referer", "商户申请H5时提交的授权域名"); //例如 http://www.baidu.com
iOS版问题
健康状态报告页面使用微信支付，支付成功或取消时使用Safari浏览器自动打开回调地址。
解决方法： WebView发起微信请求时修改请求的Referer和设置URL Types。

API接口集成方式
6.1. 舌象特征API
舌象特征API
API介绍
舌象特征API根据用户传入的舌象图片，使用AI分析出舌色、苔色、苔色、舌形、津液和舌下络脉等舌象特征。
舌象特征API完整调用流程包括：舌象预判接口、舌象特征接口和结果回调。
舌象特征API调用接口均需获取access_token。

6.1.1. 开发流程
接口调用流程描述
上图分为预判舌象接口和确认提交检测接口调用，都需要携带access_token，它的获取方式在“授权接口”章节中介绍；
预判舌象接口调用可以传入舌面图、舌下图、第三方单据流水号和结果接收地址参数，会立即响应上传成功与否；预判结果则会异步通知到结果接收地址，异步通知每隔1秒通知一次共计通知3次直到响应success则不再通知。建议您在预判结果为合格时，再调用确认提交检测接口；
确认提交检测接口需传入年龄、性别和预判的第三方单据流水号参数，会立即响应上传成功与否（成功的则检测并计费）；检测结果则会异步通知到结果接收地址，异步通知每隔1秒通知一次共计通知3次直到响应success则不再通知；
检测结果分为：最终结果和错误提示。

6.1.2. 舌象预判接口
舌象预判接口
接口描述
此接口用于预判舌象是否合格。建议预判舌象是合格时，再去调用“舌诊接口”接口。
此接口会立即响应上传成功与否；预判结果通过“结果回调”接口接收。
接口说明
请求地址： https://www.ai-tongue.com/backend/interfacesvc/i/tongue/secret/task/pre
请求头：Authorization： Bearer {access_token}
Authorization 是请求头名称；
Bearer {access_token} 是请求头的值；{access_token} 是授权令牌，从“授权接口”获取。
请求方式： POST
请求参数
使用form-data方式传参。
参数名	变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
签名	signature	String	是	对outId进行RSA签名后得到的字符串。签名工具请参考“资源下载”
舌面/舌下图片类型	imageType	Number	否	1：文件对象
2：网络图片地址，支持http/https
默认是1
舌面图片	images	File	否	imageType=1时必传
舌下图片	backImages	File	否	imageType=1时有效
舌面图片	imageUrl	String	否	imageType=2时必传
舌下图片	backImageUrl	String	否	imageType=2时有效
检测结果接收地址	returnUrl	String	是	支持http/https，需要互联网访问
请求示例
Postman导出的请求示例如下，您也可以导入Postman后查看
{
 "info": {
     "_postman_id": "0487766a-0f83-4f7a-af8a-308581068c98",
     "name": "Demo_舌象预判接口",
     "schema": "https://schema.getpostman.com/json/collection/v2.1.0/collection.json"
 },
 "item": [
     {
         "name": "舌象预判接口",
         "request": {
             "auth": {
                 "type": "bearer",
                 "bearer": [
                     {
                         "key": "token",
                         "value": "eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJleHAiOjE2MTgyMTUxMDMsInVzZXJfbmFtZSI6InRlc3RBcHAiLCJqdGkiOiJlMDFjN2Y1Mi1kNDdlLTQ0ZjktYmVjYi1hNWIxMTg3NjJjZjAiLCJjbGllbnRfaWQiOiJ0ZXN0QXBwIiwic2NvcGUiOlsiKiJdfQ.awzQc-PyA-S6OQ1Oz4rP4fZAC5fRxI8sPpKtFHW2PeA",
                         "type": "string"
                     }
                 ]
             },
             "method": "POST",
             "header": [],
             "body": {
                 "mode": "formdata",
                 "formdata": [
                     {
                         "key": "images",
                         "type": "file",
                         "src": "/C:/Users/admin/Desktop/c868f2b0-34b6-45de-900e-f70d5ec84396.png"
                     },
                     {
                         "key": "outId",
                         "value": "100",
                         "type": "text"
                     },
                     {
                         "key": "returnUrl",
                         "value": "http://k218d99927.iask.in/constitution/pre/resultReturn",
                         "type": "text"
                     },
                     {
                         "key": "signature",
                         "value": "tC6z8HoXwVp0gyHdqaDkVrlxcL9nN8MJyC9TvZ31dE/SsThNpqvGNxvVkA0iA1dYw4meB9NpSVlfuIOqa22UbRXei8T3Bg4REm+C0HdQJEnXtbgWlFpR0XmQMeWpSHDqZ3AekwPHtkv5ZUNSa0+OCIw4pvrUrfUnuweJiPQmGEY=",
                         "type": "text"
                     },
                     {
                         "key": "backImages",
                         "type": "file",
                         "src": "/C:/Users/admin/Desktop/c868f2b0-34b6-45de-900e-f70d5ec84396.jpg"
                     }
                 ]
             },
             "url": {
                 "raw": "https://www.ai-tongue.com/backend/interfacesvc/i/tongue/secret/task/pre",
                 "protocol": "https",
                 "host": [
                     "www",
                     "ai-tongue",
                     "com"
                 ],
                 "path": [
                     "backend",
                     "interfacesvc",
                     "i",
                     "tongue",
                     "secret",
                     "task",
                     "pre"
                 ]
             }
         },
         "response": []
     }
 ]
}
响应参数
参数名	变量	类型	必填	描述
错误码	code	Number	是	code为0表示成功；code不为0表示错误
提示信息	msg	String	是	code为0时，此字段是“成功”；code不为0时，此字段是错误提示信息
数据	data	Object	否	{} 或 []
响应示例
成功的例子

{
 "code": 0,
 "msg": "成功"
}
失败的例子

{
 "code": 2609002,
 "msg": "第三方单据唯一标识已存在"
}

6.1.3. 舌象特征接口
舌象特征接口
接口描述
此接口用于上传舌象检测。
此接口会立即响应上传成功与否；检测结果通过“结果回调”接口接收。
此接口调用需要先调用“舌象预判接口”。
接口说明
请求地址： https://www.ai-tongue.com/backend/interfacesvc/i/tongue/secret/task/do/character
请求头：Authorization： Bearer {access_token}
Authorization 是请求头名称；
Bearer {access_token} 是请求头的值；{access_token} 是授权令牌，从“授权接口”获取。
请求方式： POST
请求参数
使用form-data方式传参。
参数名	变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
签名	signature	String	是	对outId进行RSA签名后得到的字符串。签名工具请参考“资源下载”
年龄和性别加密数据	encryptData	String	否	原文形如：{"age":20,"sex":1}，然后使用AES算法对其加密得到的字符串。加密算法请参考“资源下载”。
1、age(Integer)：（不必填）年龄；大于等于0
2、sex(Integer)：（不必填）性别；0：未知，1：男，2：女
请求示例
无

响应参数
参数名	变量	类型	必填	描述
错误码	code	Number	是	code为0表示成功；code不为0表示错误
提示信息	msg	String	是	code为0时，此字段是“成功”；code不为0时，此字段是错误提示信息
数据	data	Object	否	code为0时，此字段是数字，代表预计完成检测剩余秒数；code不为0时，此字段是空
响应示例
成功的例子

{
 "code": 0,
 "data": 20,
 "msg": "成功"
}
失败的例子

{
 "code": 2609002,
 "msg": "第三方单据唯一标识已存在"
}

6.1.4. 结果回调
结果回调
接口描述
此接口由第三方提供，用于接收平台返回的结果数据。
一般来说，平台返回给第三方数据时每隔1秒通知一次，共计通知3次，直到响应success则不再通知。
接口说明
请求地址： 第三方提供
请求头：无
请求方式： POST
请求参数
使用form-data方式传参。
  参数名  
变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
签名	signature	String	是	对outId进行RSA签名后得到的字符串。这里使用的是平台私钥签名，第三方应该使用平台公钥（rsaPublicKey）验签
结果加密数据	encryptData	String	是	需要使用AES进行解密。解密算法请参考“资源下载”。根据原文中returnType字段的值不同，则返回类型不同，详见下面请求示例
encryptData对应原文中returnType字段各个值的含义如下表：
  类型  
含义
returnType=31	预判是舌象
returnType=32	预判不是舌象
returnType=1	最终结果
returnType=2	错误提示
请求示例
1、预判是舌象
原文示例
{
    "outId": "1",
    "returnType": 31
}
参数说明
  参数名  
变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
返回类型	returnType	Number	是	returnType=31表示预判是舌象。可以继续调用“舌诊接口”
2、预判不是舌象
原文示例
{
    "error": {
        "code": 206,
        "msg": "图片不是舌下（请拍摄带有舌下的、清晰的彩色照！）"
    },
    "outId": "2",
    "returnType": 32
}
参数说明
  参数名  
变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
返回类型	returnType	Number	是	returnType=32表示预判不是舌象。此时不建议再调用“舌诊接口”，因为仅仅会得出同样的错误提示
错误信息	error	Object	是	详见错误码列举
3、最终结果
原文示例
{
    "outId": "11",
    "result": {
        "bodyfluidNames": "正常",
        "colorOfMossCurveSort": 1,
        "colorOfMossDescribe": "舌苔呈现白色。</br>可见于正常人，也主表证、寒证。</br>",
        "colorOfMossNames": "白苔",
        "colorOfTongueCurveSort": 0,
        "colorOfTongueDescribe": "【淡白舌-舌象特征】舌色较正常舌色（淡红舌）浅淡，白多红少，甚至全无血色。</br>【淡白舌-病理意义】主气血两虚、阳虚。</br>",
        "colorOfTongueNames": "淡白舌",
        "mossNames": "正常",
        "ossOriImgUrl": "https://td-platform-ori.oss-cn-hangzhou.aliyuncs.com/ai/tonguediagnosis/2020/10/96b7c268-d860-4c36-a26a-ffac2fbabd1d.jpg",
        "ossSplitBackImgUrl": "https://td-platform-ori-back.oss-cn-hangzhou.aliyuncs.com/ai/tonguediagnosis/2020/10/96b7c268-d860-4c36-a26a-ffac2fbabd1d.png",
        "ossSplitImgUrl": "https://td-platform-split.oss-cn-hangzhou.aliyuncs.com/ai/tonguediagnosis/2020/10/96b7c268-d860-4c36-a26a-ffac2fbabd1d.png",
        "shapeOfTongueDescribe": "舌体浮胖娇嫩，纹理细腻。舌色浅淡为淡嫩舌，舌色偏红为红嫩舌。</br>嫩舌多主虚证。淡嫩舌多见于气血虚弱，脏腑功能减退的虚证。红嫩舌提示气阴两虚。</br>舌体比正常舌大，伸舌满口，可伴有舌边齿痕。舌体肿大满嘴，甚至不能闭口。伸出难以缩回，称为肿胀舌。</br>胖大舌多主水湿痰饮内停。肿胀舌多主湿热、热毒上壅。</br>",
        "shapeOfTongueNames": "嫩,胖"
    },
    "returnType": 1
}
参数说明
基础参数
  参数名  
变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
返回类型	returnType	Number	是	returnType=1表示是最终结果
结果	result	Object	是	详见结果参数
结果参数
  参数名  
变量	类型	必填	描述
津液	bodyfluidNames	String	是	-
津液描述	bodyfluidDescribe	String	否	-
苔色	colorOfMossNames	String	否	-
苔色描述	colorOfMossDescribe	String	否	-
舌色	colorOfTongueNames	String	是	-
舌色描述	colorOfTongueDescribe	String	否	-
苔质	mossNames	String	是	-
苔质描述	mossDescribe	String	否	-
舌形	shapeOfTongueNames	String	是	-
舌形描述	shapeOfTongueDescribe	String	否	-
络脉	veinNames	String	否	-
络脉描述	veinDescribe	String	否	-
舌面原图矫正图	ossOriImgUrl	String	是	舌诊平台自动调整舌象为纵向的图，方便查看。可不使用
舌面分割图	ossSplitImgUrl	String	是	-
舌下分割图	ossSplitBackImgUrl	String	否	-
4、错误提示
原文示例
{
    "error": {
        "code": 201,
        "msg": "图片过暗"
    },
    "outId": "11",
    "returnType": 2
}
参数说明
  参数名  
变量	类型	必填	描述
第三方单据流水号	outId	String	是	第三方唯一标识
返回类型	returnType	Number	是	returnType=2表示是错误提示
错误信息	error	Object	是	详见 API接口回调错误码

6.1.5. 示例代码
示例代码
目前Java版提供完整接口调用示例，对JavaScript、PHP、Python和.NET提供AES和RSA工具类

Java版例子
https://gitee.com/ai-tongue/ai-tongue-java/blob/master/src/main/java/com/mxjsxz/demo/controller/pre/DemoPreCharacterController.java
DemoPreCharacterController.java

package com.mxjsxz.demo.controller.pre;

import com.mxjsxz.demo.constants.AiTongueConstant;
import com.mxjsxz.demo.model.form.TongueTaskEncryptDataForm;
import com.mxjsxz.demo.model.vo.ResultVO;
import com.mxjsxz.demo.model.vo.ReturnVO;
import com.mxjsxz.demo.model.vo.TongueReturnVO;
import com.mxjsxz.demo.properties.AiTongueProperties;
import com.mxjsxz.demo.service.IRestTemplateService;
import com.mxjsxz.demo.utils.AesSimpleUtil;
import com.mxjsxz.demo.utils.JsonUtil;
import com.mxjsxz.demo.utils.RsaSimpleUtil;
import org.apache.commons.lang3.StringUtils;
import org.slf4j.Logger;
import org.slf4j.LoggerFactory;
import org.springframework.beans.factory.annotation.Autowired;
import org.springframework.util.LinkedMultiValueMap;
import org.springframework.util.MultiValueMap;
import org.springframework.web.bind.annotation.PostMapping;
import org.springframework.web.bind.annotation.RequestMapping;
import org.springframework.web.bind.annotation.RestController;

import java.io.File;
import java.util.HashMap;
import java.util.Map;

import static com.mxjsxz.demo.constants.AiTongueConstant.SUCCESS;

/**
 * 舌象特征API
 *
 * @author xuwenbing
 * @date 2021-03-17
 */
@RestController
@RequestMapping("character/pre")
public class DemoPreCharacterController {
    private Logger log = LoggerFactory.getLogger(DemoPreCharacterController.class);
    private final AiTongueProperties aiTongueProperties;
    private final IRestTemplateService restTemplateService;

    @Autowired
    public DemoPreCharacterController(AiTongueProperties aiTongueProperties, IRestTemplateService restTemplateService) {
        this.aiTongueProperties = aiTongueProperties;
        this.restTemplateService = restTemplateService;
    }

    /**
     * 阶段一：验证舌象
     *
     * @return
     */
    @PostMapping("index")
    public String index() throws Exception {
        // 1.获取accesstoken
        String accesstoken = this.getAccessToken(aiTongueProperties.getDevId(), aiTongueProperties.getDevSecret());
        if (StringUtils.isBlank(accesstoken)) {
            return AiTongueConstant.ERROR;
        }
        Map<String, String> headers = new HashMap<>();
        headers.put("Authorization", "Bearer " + accesstoken);

        // 2.准备待检测的数据：第三方单据id、舌面图片、舌下图片、年龄、性别和结果接收地址
        Integer outId = 1;
        File imageFile = new File(this.getClass().getClassLoader().getResource("static/tongue.jpg").getFile());
        File backImageFile = new File(this.getClass().getClassLoader().getResource("static/tongueBack.jpg").getFile());
        String returnUrl = "https://your.domain/character/pre/resultReturn"; //您的结果接收地址

        // 3.签名数据
        String signature = RsaSimpleUtil.sign(Integer.toString(outId), aiTongueProperties.getDevRsaPrivateKey());

        // 4.上传检测
        MultiValueMap<String, Object> params = new LinkedMultiValueMap<>();
        params.add("outId", outId);
        params.add("returnUrl", returnUrl);
        params.add("signature", signature);
        params.add("images", restTemplateService.getFileSystemResource(imageFile));
        params.add("backImages", restTemplateService.getFileSystemResource(backImageFile));
        // 开启下面的代码表示使用网络舌象图片,支持http/https
//        params.add("imageType", 2);
//        params.add("imageUrl", "https://your.domaim/tongue.jpg");
//        params.add("backImageUrl", "https://your.domaim/tongueBack.jpg");

        // 当resultVO.code=0表示上传成功：
        // （1）检测的结果会回传到您设置的returnUrl上
        ResultVO resultVO = restTemplateService.postForObject(aiTongueProperties.getPreTongueUrl(), headers, params, ResultVO.class);
        log.info("index:{}", JsonUtil.toJson(resultVO));
        return AiTongueConstant.OK;
    }

    /**
     * 阶段二：确认提交检测
     *
     * @return
     */
    @PostMapping("taskCharacter")
    public String taskCharacter() throws Exception {
        // 1.获取accesstoken
        String accesstoken = this.getAccessToken(aiTongueProperties.getDevId(), aiTongueProperties.getDevSecret());
        if (StringUtils.isBlank(accesstoken)) {
            return AiTongueConstant.ERROR;
        }
        Map<String, String> headers = new HashMap<>();
        headers.put("Authorization", "Bearer " + accesstoken);

        // 2.准备待检测的数据：第三方单据id、舌面图片、舌下图片、年龄、性别和结果接收地址
        Integer outId = 1;
        Integer age = 20; // 大于等于0
        Integer sex = 1; // 0：未知 1：男 2：女

        // 3.加密和签名数据
        String signature = RsaSimpleUtil.sign(Integer.toString(outId), aiTongueProperties.getDevRsaPrivateKey());
        String sourceData = JsonUtil.toJson(new TongueTaskEncryptDataForm(age, sex));
        String encryptData = AesSimpleUtil.encrypt(sourceData, aiTongueProperties.getAesKey());

        // 4.上传检测
        MultiValueMap<String, Object> params = new LinkedMultiValueMap<>();
        params.add("outId", outId);
        params.add("signature", signature);
        params.add("encryptData", encryptData);
        // 当resultVO.code=0表示上传成功：
        // （1）resultVO.data表示预计等待检测时间，
        // （2）检测的结果会回传到您设置的returnUrl上
        ResultVO resultVO = restTemplateService.postForObject(aiTongueProperties.getPreTongueCharacterTaskUrl(), headers, params, ResultVO.class);
        log.info("taskCharacter:{}", JsonUtil.toJson(resultVO));
        return AiTongueConstant.OK;
    }

    /**
     * 2、结果接收地址
     *
     * @param returnVO
     * @return
     */
    @PostMapping("resultReturn")
    public String resultReturn(ReturnVO returnVO) throws Exception {
        log.info("character resultReturn：{}", JsonUtil.toJson(returnVO));
        // 1. 验证签名
        boolean verify = RsaSimpleUtil.verify(returnVO.getOutId(), returnVO.getSignature(), aiTongueProperties.getRsaPublicKey());
        if (verify) {
            // 2. 只有验签通过后才进行业务操作
            // 3. 解密数据
            String decryptData = AesSimpleUtil.decrypt(returnVO.getEncryptData(), aiTongueProperties.getAesKey());
            // 4. decryptData可以转化为TongueReturnVO对象,具体每个字段含义见TongueReturnVO
            // 其中returnType表示返回结果的类型
            // returnType=1 说明返回的最终体质结果，此时您可以保存结果并返回给用户
            // returnType=2 说明返回的失败提示信息，此时您可以反馈给用户
            // returnType=31 预判为合法图片，此时您可以调用“阶段二：确认提交检测”接口
            // returnType=32 预判为不合法图片，此时您可以反馈给用户，并且不推荐继续调用“阶段二：确认提交检测”接口
            log.info("character decryptData：{}", decryptData);
            TongueReturnVO tongueReturnVO = JsonUtil.parseObject(decryptData, TongueReturnVO.class);
            return SUCCESS;
        }
        log.info("验证签名失败");
        return AiTongueConstant.ERROR;
    }

    /**
     * 获取access_token（获取后建议缓存，一般30分钟有效）
     *
     * @param devId
     * @param devSecret
     * @return
     */
    private String getAccessToken(String devId, String devSecret) {
        MultiValueMap<String, Object> params = new LinkedMultiValueMap<>();
        params.add("devid", devId);
        params.add("devsecret", devSecret);
        ResultVO accessTokenResult = restTemplateService.postForObject(aiTongueProperties.getGetTokenUrl(), params, ResultVO.class);
        log.info("access_token result:{}", JsonUtil.toJson(accessTokenResult));
        if (accessTokenResult.getCode() != 0) {
            return null;
        }
        return ((Map) accessTokenResult.getData()).get("access_token").toString();
    }
}

JavaScript版例子
https://gitee.com/ai-tongue/ai-tongue-nodejs

PHP版例子
https://gitee.com/ai-tongue/ai-tongue-php

Python版例子
https://gitee.com/ai-tongue/ai-tongue-python
aes.py

#  aes-128-ecb PKCS5Padding
import base64

from Crypto.Cipher import AES


def AES_encrypt(secret_key, data):
    """
    :param secret_key [str] : 加密秘钥
    :param data [str] : 需要加密数据
    :return   [str] :
    """
    BLOCK_SIZE = 16  # Bytes
    # 数据进行 PKCS5Padding 的填充
    pad = lambda s: (s + (BLOCK_SIZE - len(s) % BLOCK_SIZE) * chr(BLOCK_SIZE - len(s) % BLOCK_SIZE))
    raw = pad(str(data))
    # 通过key值，使用ECB模式进行加密
    cipher = AES.new(base64.b64decode(secret_key), AES.MODE_ECB)
    # 得到加密后的字节码
    encrypted_text = cipher.encrypt(bytes(raw, encoding='utf-8'))
    # 字节码转换成十六进制  再转成 字符串
    # encrypted_text_hex = str(b2a_hex(encrypted_text), encoding='utf-8')
    encrypted_text_hex = base64.b64encode(encrypted_text).decode("utf-8")
    return encrypted_text_hex


def AES_decrypt(secret_key, encrypted_text_hex):
    """
    :param secret_key [str] : 加密秘钥
    :param encrypted_text_hex [str]: # 加密后的 data 字符串
    :return [str]:
    """
    # 去掉 PKCS5Padding 的填充
    unpad = lambda s: s[:-ord(s[len(s) - 1:])]
    # 通过 key 值进行
    cipher = AES.new(base64.b64decode(secret_key), AES.MODE_ECB)
    # data_response = unpad(cipher.decrypt(a2b_hex(encrypted_text_hex))).decode('utf8')
    data_response = unpad(cipher.decrypt(base64.b64decode(encrypted_text_hex))).decode('utf8')
    return data_response


if __name__ == '__main__':
    secret_key = "xxxxxxxxxxxxxxxxxxxxxxxx"  # 秘钥 （需要16位,base64方式24位）
    dataEncrypt = AES_encrypt(secret_key, "123456789")  # 加密
    print(dataEncrypt)  # 打印加密后的数据
    data = AES_decrypt(secret_key, dataEncrypt)  # 解密
    print(data)  # 打印解密后的数据

rsa.py

import base64

import Crypto.Signature.PKCS1_v1_5 as sign_PKCS1_v1_5  # 用于签名/验签
from Crypto import Random
from Crypto.Cipher import PKCS1_v1_5  # 用于加密
from Crypto.Hash import MD5
from Crypto.PublicKey import RSA

# 公钥
PUBLIC_KEY_STR = "xxxxxx"
# 私钥
PRIVATE_KEY_STR = "xxxxxx"
# 编码
UTF8 = 'utf-8'


def handle_key(keystr, type=1):
    '''
        公钥格式pem，处理成以-----BEGIN PUBLIC KEY-----开头，-----END PUBLIC KEY-----结尾的格式
        type==1:公钥  type==2：私钥
    '''
    start = '-----BEGIN PUBLIC KEY-----\n'
    end = '-----END PUBLIC KEY-----'
    if type == 2:
        start = '-----BEGIN RSA PRIVATE KEY-----\n'
        end = '-----END RSA PRIVATE KEY-----'
    result = ''
    # 分割key，每64位长度换一行
    divide = int(len(keystr) / 64)
    divide = divide if (divide > 0) else divide + 1
    line = divide if (len(keystr) % 64 == 0) else divide + 1
    for i in range(line):
        result += keystr[i * 64:(i + 1) * 64] + '\n'
    result = start + result + end
    return result


def rsaEncrypt(plain_text):
    '''
        公钥加密
    '''
    # 加载公钥
    public_key_pem = handle_key(PUBLIC_KEY_STR)
    public_key = RSA.import_key(public_key_pem)

    # 公钥加密
    cipher_pub_obj = PKCS1_v1_5.new(public_key)
    secret_bytes = cipher_pub_obj.encrypt(plain_text.encode(encoding=UTF8))
    secret_b64 = base64.b64encode(secret_bytes)
    secret_b64_str = str(secret_b64, encoding=UTF8)
    return secret_b64_str


def rsaDecrypt(secret_b64_str):
    '''
        私钥解密
    '''
    # 加载私钥
    private_key_pem = handle_key(PRIVATE_KEY_STR, 2)
    private_key = RSA.import_key(private_key_pem)

    secret_bytes = base64.b64decode(secret_b64_str)
    # 私钥解密
    cipher_pri = PKCS1_v1_5.new(private_key)
    plain_byte = cipher_pri.decrypt(secret_bytes, Random.new().read)
    plain_text = plain_byte.decode(UTF8)
    return plain_text


def sign(plain_text):
    '''
        签名
    '''
    # 加载私钥
    private_key_pem = handle_key(PRIVATE_KEY_STR, 2)
    private_key = RSA.import_key(private_key_pem)

    # md5withrsa
    signer = sign_PKCS1_v1_5.new(private_key)
    hash_obj = MD5.new(plain_text.encode(UTF8))

    signature = base64.b64encode(signer.sign(hash_obj)).decode(UTF8)
    return signature


def verify(plain_text, signature):
    '''
        验签
    '''
    # 加载公钥
    public_key_pem = handle_key(PUBLIC_KEY_STR)
    public_key = RSA.import_key(public_key_pem)

    verifier = sign_PKCS1_v1_5.new(public_key)

    # md5withrsa
    hash_obj = MD5.new(plain_text.encode(UTF8))

    is_verify = verifier.verify(hash_obj, base64.b64decode(signature))
    return is_verify


if __name__ == '__main__':
    plain_text = 'hello world!'
    print('原文内容', plain_text)
    secret_content = rsaEncrypt(plain_text)
    print('加密内容', secret_content)
    content = rsaDecrypt(secret_content)
    print('解密内容', content)

    signature = sign(plain_text)
    print('验签内容', plain_text)
    print('签名内容', signature)
    is_verify = verify(plain_text, signature)
    print('验签结果', is_verify)

.NET版例子
https://gitee.com/ai-tongue/ai-tongue-.net

6.1.6. 常见问题
常见问题
调用接口时，系统返回 “验签错误，请确认开发者rsa私钥（devRsaPrivateKey）正确”
先检查是不是使用开发参数中的devRsaPrivateKey字段进行签名操作的。
再检查是不是使用的是示例代码中的RSA工具类。
调用接口时，系统返回 “解密错误，请确认aeskey正确”
先检查是不是使用开发参数中的aeskey字段进行加密操作的。
再检查是不是使用的是示例代码中的AES工具类。
验签系统的回调数据失败
检查是不是使用开发参数中的rsaPublicKey字段进行验签操作的。
如果系统的回调数据包含“%2B”或“%2F”之类字样，请先使用URLDECODE后再进行验签操作。
解密系统的回调数据失败
检查是不是使用开发参数中的aesKey字段进行解密操作的。
如果系统的回调数据包含“%2B”或“%2F”之类字样，请先使用URLDECODE后再进行解密操作。
调用接口是什么时候开始计费的？
调用舌象特征接口，并系统返回成功时计费；调用舌象预判接口不会计费。所以推荐先调用舌象预判接口，预判为合格时再调用舌象特征接口。
如何将API返回的中文数据翻译成英文？
目前来说，翻译工作需要接口调用方来做，详见翻译说明。
