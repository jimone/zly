### 菜单获取

```javascript
参数：
{
    'controller':'card',
    'action':'index',
    'option':'menu'
}
返回：
{
    "msg": "成功",
    "code": true,
    "data": {
        "interface": {
            "id": "2",
            "member": "4",
            "title": "众旅云",
            "logo": "http://wx.qlogo.cn/mmopen/PLc9fhw8iashRwVh0RnTAPKty3I92cDzKzwsmSbv8tYplCB3Wj4T5rfuOE2nGC8UxDnibrhN7FXcrYkRxQdoYltZ5zjwgOmZna/0",
            "service": "2",
            "appuser": "gh_dd71d4eef1bf",
            "qrcode_url": "http://mmbiz.qpic.cn/mmbiz/7aiaADrlRXiar2iaZ0VJQI5fficEfFs9SLmtw95laC6icGqjgv1GbfsRR2n6tbTer3ia0aDzjjbL31ClE31ibpBwibABtg/0"
        },
        "menu": [
            {
                "id": "2",
                "member_id": "4",
                "name": "用户信息",
                "url": "www.baidu.com",
                "order": "12",
                "dateline": "1464329680"
            },
            {
                "id": "3",
                "member_id": "4",
                "name": "订单管理",
                "url": "www.world.com",
                "order": "5",
                "dateline": "1464329720"
            }
        ]
    }
}
```

### 年卡列表
```javascript
参数：
{
    'controller': 'card',
    'action': 'index',
    'option': 'cardList'
}
返回：
{
    "msg": "成功",
    "code": true,
    "data": {
        "interface": {'略'},
        "cardList": [
            {
                "id": "3",
                "member_id": "4",
                "image": "http://testtmpimage.b0.upaiyun.com/201605/03/146224483062210259.jpg",//年卡图片
                "configure": "360500*",
                "name": "新余旅游年卡",
                "free": "150.00",//年卡线下价格
                "delete": "0",
                "dateline": "1464224290",//时间
                "money": "90.99",//年卡线上价格
                "back_image": "http://testtmpimage.b0.upaiyun.com/201605/13/146312803163893373.jpg",//背部图片
                "type": "1", //排版模式1为竖版,2为横板
                "now_sale": 0.2 //年卡线上折扣
            },
            {
                "id": "5",
                "member_id": "4",
                "image": "http://testtmpimage.b0.upaiyun.com/201605/20/146373482392500255.jpg",
                "configure": "",
                "name": "测试",
                "free": "0.10",
                "delete": "0",
                "dateline": "1463734823",
                "money": "0.10",
                "back_image": "http://testtmpimage.b0.upaiyun.com/201605/20/146373482405790041.jpg",
                "type": "1",
                "now_sale": 0.1
            }
        ],
    }
}
```

### 年卡详情
```javascript
参数
{
    'controller':'card',
    'action':'detail',
    'cardId':,   //年卡id
    'option':'getDetail',
    'isDesc':   //是否获取详情（1=>获取use_desc,buy_desc（年卡使用，购买详情）      0=>不获取use_desc,buy_desc）
}
返回
{
    "msg": "成功",
    "code": true,
    "data": {
        "interface": {"略"},
        "cardRow": {
            "id": "5",
            "member_id": "4",
            "buy_desc": "略",
            "use_desc": "略",
            "configure": "",
            "name": "测试",
            "delete": "0",
            "dateline": "1464596757",
            "money": "0.10",
            "free": "0.10",
            "image": "http://testtmpimage.b0.upaiyun.com/201605/20/146373482392500255.jpg",
            "back_image": "http://testtmpimage.b0.upaiyun.com/201605/20/146373482405790041.jpg",
            "type": "1"
        },
        "saleRow": {
            "id": "18",
            "member_id": "4",
            "card_id": "5",
            "starttime": "1464579600",
            "endtime": "1464677400",
            "sale": "10",
            "delete": "0",
            "desc": "<p>说啥呢</p>",
            "isonline": "1",
            "name": "第二个测试"
        }
    }
}
```

### 年卡申请
```javascript
参数
{
    'controller':'card',
    'action':'check',
    'option':'apply',
    'tel':'',
    'IDcard':'',
    'name':'',
    'userId':'',  //可选
    'dealerId':"",
    'cardId':"",
    'gender':"",
    'id_type':"",
    'front_img':"",
    'reverse_img':"",
    'type_img':"",
}
返回
{
    "msg": "成功",
    "code": true,
    "data": {
        "interface": {'略'},
        "userId": "" 
    }
}
```


### 年卡申请流程图
![image](https://github.com/MelonYii/images/blob/6633066c8216e169c716e5bd5133d6c74a3ecbba/cardApply.png)