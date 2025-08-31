欧本随身wifi的流量查询脚本，运行于青龙面板

# --- 配置项 ---
# 在青龙面板选择-环境变量-然后添加变量名称WIFI_DEV_NOS，值就填你的设备号，多个设备号用英文 & 符号连接。
# 示例: 86825xxxx&12345xxxx
# 或者一台设备就添加一个变量都行，可以添加多个变量
DEV_NO_LIST_STRING = os.getenv('WIFI_DEV_NOS')

# WECHAT_ROBOT_WEBHOOK: 选填。企业微信机器人的 Webhook 地址，用于接收推送消息。
WECHAT_ROBOT_WEBHOOK = os.getenv('WECHAT_ROBOT_WEBHOOK')

# WXPUSHER_APP_TOKEN: 选填。WxPusher 的 AppToken。
WXPUSHER_APP_TOKEN = os.getenv('WXPUSHER_APP_TOKEN')
# WXPUSHER_UIDS: 选填。你的 WxPusher UID，多个 UID 请用英文 & 符号连接。
WXPUSHER_UIDS = os.getenv('WXPUSHER_UIDS')

# SERVERJANG_SCKEY: 选填。Server酱的 SCKEY，用于微信推送。
SERVERJANG_SCKEY = os.getenv('SERVERJANG_SCKEY')

# BARK_PUSH_URL: 选填。Bark 推送的 URL，用于 iOS 推送。
BARK_PUSH_URL = os.getenv('BARK_PUSH_URL')

# PUSHPLUS_TOKEN: 选填。PushPlus 的 Token，用于微信公众号/企业微信推送。
PUSHPLUS_TOKEN = os.getenv('PUSHPLUS_TOKEN')

# DINGTALK_WEBHOOK: 选填。钉钉机器人 Webhook 地址，用于钉钉群推送。
DINGTALK_WEBHOOK = os.getenv('DINGTALK_WEBHOOK')

# FEISHU_WEBHOOK: 选填。飞书机器人 Webhook 地址，用于飞书群推送。
FEISHU_WEBHOOK = os.getenv('FEISHU_WEBHOOK')



# 控制推送模式：
# 'full' (详细推送，并打印所有可读字段)
# 'simple' (精简推送)
# 'off' (不推送)
PUSH_MODE = 'simple'
