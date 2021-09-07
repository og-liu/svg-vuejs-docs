## 示例

> 插件默认提供了一套常用的图标集合，复制图标的 name 即可直接使用，图标下方汉字描述可用于快速搜索。

```vue
<vue-svg name="svg-tachometer" color="#42b983"></vue-svg>
```

## 常用字体图标集合

<ul class="icon-list">
    <li>
        <div class="icon tachometer"></div>
        <div class="icon-name">svg-tachometer</div>
        <div class="icon-name">数据 转速表</div>
    </li>
    <li>
        <div class="icon trade"></div>
        <div class="icon-name">svg-trade</div>
        <div class="icon-name">订单 交易</div>
    </li>
    <li>
        <div class="icon product"></div>
        <div class="icon-name">svg-product</div>
        <div class="icon-name">产品 层叠</div>
    </li>
    <li>
        <div class="icon calendar"></div>
        <div class="icon-name">svg-calendar</div>
        <div class="icon-name">活动 日历</div>
    </li>
    <li>
        <div class="icon coins"></div>
        <div class="icon-name">svg-coins</div>
        <div class="icon-name">仓储 数据库</div>
    </li>
    <li>
        <div class="icon user-tie"></div>
        <div class="icon-name">svg-user-tie</div>
        <div class="icon-name">客户 用户</div>
    </li>
    <li>
        <div class="icon store"></div>
        <div class="icon-name">svg-store</div>
        <div class="icon-name">商城 店铺</div>
    </li>
    <li>
        <div class="icon dollar"></div>
        <div class="icon-name">svg-dollar</div>
        <div class="icon-name">财务 美元</div>
    </li>
    <li>
        <div class="icon users"></div>
        <div class="icon-name">svg-users</div>
        <div class="icon-name">团队 群体</div>
    </li>
    <li>
        <div class="icon boxes"></div>
        <div class="icon-name">svg-boxes</div>
        <div class="icon-name">联盟 盒子</div>
    </li>
    <li>
        <div class="icon building"></div>
        <div class="icon-name">svg-building</div>
        <div class="icon-name">企业 建筑</div>
    </li>
    <li>
        <div class="icon cogs"></div>
        <div class="icon-name">svg-cogs</div>
        <div class="icon-name">系统 齿轮</div>
    </li>
    <li>
        <div class="icon phone"></div>
        <div class="icon-name">svg-phone</div>
        <div class="icon-name">手机</div>
    </li>
    <li>
        <div class="icon desktop"></div>
        <div class="icon-name">svg-desktop</div>
        <div class="icon-name">电脑</div>
    </li>
</ul>

<style>
* {padding: 0; margin: 0; list-style: none;}
img { display: block; }
.icon-list {
    margin-top: 20px;
    overflow: hidden;
    padding: 0!important;
    border: 1px solid #eaeefb;
    border-radius: 4px;
    display: flex;
    flex-wrap: wrap;
}
.icon-list li {
    width: calc(100% / 9 + 1px);
    height: 120px;
    color: #666;
    font-size: 14px;
    font-weight: 900;
    border-right: 1px solid #eee;
    border-bottom: 1px solid #eee;
    margin-right: -1px;
    margin-bottom: -1px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    cursor: pointer;
}
.icon {
    width: 34px;
    height: 34px;
    margin-bottom: 10px;
    background-repeat: no-repeat!important;
    background-size: 100% 100%!important;
}

.icon-list li:hover {
    color: #5cb6ff;
}
</style>

<style>
/* 数据 */
.tachometer {
    background: url("iconfont/default/tachometer.svg");
    
}
.icon-list li:hover .tachometer {
    background-image: url("iconfont/hover/tachometer.svg");
}
/* 订单 */
.trade {
    background: url("iconfont/default/trade.svg");
    
}
.icon-list li:hover .trade {
    background-image: url("iconfont/hover/trade.svg");
}
/* 产品 */
.product {
    background: url("iconfont/default/product.svg");
    
}
.icon-list li:hover .product {
    background-image: url("iconfont/hover/product.svg");
}
/* 活动 */
.calendar {
    background: url("iconfont/default/calendar.svg");
    
}
.icon-list li:hover .calendar {
    background-image: url("iconfont/hover/calendar.svg");
}
/* 仓储 */
.coins {
    background: url("iconfont/default/coins.svg");
    
}
.icon-list li:hover .coins {
    background-image: url("iconfont/hover/coins.svg");
}
/* 客户 */
.user-tie {
    background: url("iconfont/default/user-tie.svg");
    
}
.icon-list li:hover .user-tie {
    background-image: url("iconfont/hover/user-tie.svg");
}
/* 商城 */
.store {
    background: url("iconfont/default/store.svg");
    
}
.icon-list li:hover .store {
    background-image: url("iconfont/hover/store.svg");
}
/* 财务 */
.dollar {
    background: url("iconfont/default/dollar.svg");
    
}
.icon-list li:hover .dollar {
    background-image: url("iconfont/hover/dollar.svg");
}
/* 团队 */
.users {
    background: url("iconfont/default/users.svg");
    
}
.icon-list li:hover .users {
    background-image: url("iconfont/hover/users.svg");
}
/* 联盟 */
.boxes {
    background: url("iconfont/default/boxes.svg");
    
}
.icon-list li:hover .boxes {
    background-image: url("iconfont/hover/boxes.svg");
}
/* 企业 */
.building {
    background: url("iconfont/default/building.svg");
    
}
.icon-list li:hover .building {
    background-image: url("iconfont/hover/building.svg");
}
/* 系统 */
.cogs {
    background: url("iconfont/default/cogs.svg");
    
}
.icon-list li:hover .cogs {
    background-image: url("iconfont/hover/cogs.svg");
}
/* 手机 */
.phone {
    background: url("iconfont/default/phone.svg");
    
}
.icon-list li:hover .phone {
    background-image: url("iconfont/hover/phone.svg");
}
/* 电脑 */
.desktop {
    background: url("iconfont/default/desktop.svg");
    
}
.icon-list li:hover .desktop {
    background-image: url("iconfont/hover/desktop.svg");
}
</style>
