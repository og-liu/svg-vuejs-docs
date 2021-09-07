<ul class="icon-list">
    <li>
        <div class="icon tachometer"></div>
        <div class="icon-name">svg-tachometer</div>
        <div class="icon-name">数据 转速表SHG</div>
    </li>
</ul>

<style>
/* 数据 */
.tachometer {
    background: url("iconfont/default/tachometer.svg");
    
}
.icon-list li:hover .tachometer {
    background-image: url("iconfont/hover/tachometer.svg");
}
</style>

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
