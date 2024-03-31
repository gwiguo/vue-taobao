<template>
	<div class="index-page">
		<div class="top-container">
			<h1 class="logo">
				<a href="javascript:;"></a>
			</h1>
			<div class="search-container">
				<div class="input-container">
					<input type="text" placeholder="零食" />
					<button>搜索</button>
				</div>
				<div class="search-hots">
					<a href="javascript:;">手机</a>
					<a href="javascript:;">货架</a>
					<a href="javascript:;">空调</a>
					<a href="javascript:;">笔记本电脑</a>
					<a href="javascript:;">女装</a>
					<a href="javascript:;">男鞋</a>
					<a href="javascript:;">床</a>
					<a href="javascript:;">沙发</a>
					<a href="javascript:;">电脑主机</a>
					<a href="javascript:;">apple</a>
					<a href="javascript:;">vivo</a>
					<a href="javascript:;">小米</a>
					<a href="javascript:;">瓷砖</a>
				</div>
			</div>
		</div>
        <div class="main clearfix">
            <div class="pick-header">猜你喜欢</div>
            <div class="pick-container">
                <a class="item" href="javascript:;" v-for="(item,index) in 50" :key="index">
                    <img
                        src="https://img.alicdn.com/bao/uploaded/i1/374196816/O1CN01Ujhnru20DmUXDcZq9_!!374196816.jpg"
                        alt=""
                    />
                    <div class="info">阿四出品 农家古田银耳干货 白木耳糯耳雪耳无硫桃胶莲子羹250克</div>
                    <div class="price-wrapper">
                        <span class="price-unit">¥</span>
                        <span class="price-value">35.6</span>
                        <span class="price-sale">500+人购买</span>
                    </div>
                </a>
            </div>
        </div>
	</div>
</template>

<script>
export default {
	name: "home"
};
</script>

<style lang="less">
.index-page {
	margin: 0 auto;
	width: 1400px;
	.top-container {
		display: flex;
		box-sizing: border-box;
		margin: 0 auto;
		margin-top: 20px;
		height: 72px;
		h1.logo {
			margin-right: 20px;
			width: 190px;
			height: 72px;
			a {
				display: block;
				padding-top: 72px;
				width: 142px;
				height: 0;
				overflow: hidden;
				text-indent: -9999px;
				background: url(//gw.alicdn.com/imgextra/i3/O1CN01uRz3de23mzWofmPYX_!!6000000007299-2-tps-143-59.png) 0
					0 no-repeat;
				background-size: contain;
				background-position: center;
			}
		}
		.search-container {
			.input-container {
				padding: 2px;
				display: flex;
				align-items: center;
				justify-content: end;
				width: 972px;
				height: 38px;
				border: 2px solid #ff5000;
				border-radius: 8px;
				input {
					box-sizing: border-box;
					flex: 1 1 auto;
					height: 38px;
					line-height: 38px;
					border: none;
					outline: none;
					font-size: 16px;
					padding-left: 20px;
					color: #50607a;
				}
				button {
					margin-left: 10px;
					height: 34px;
					width: 72px;
					border: none;
					color: #fff;
					font-size: 16px;
					font-weight: 700;
					cursor: pointer;
					border-radius: 4px;
					background: #ff5000;
				}
			}
			.search-hots {
				margin-top: 10px;
				margin-left: 10px;
				a {
					margin-right: 8px;
					color: #50607a;
					font-size: 12px;
				}
			}
		}
	}
    .main{
        margin-top: 20px;
        padding-top: 20px;
        border-radius: 16px;
        background-color: #fff;
        .pick-header {
            // margin-top: 40px;
            margin-bottom: 20px;
            margin-left: 26px;
            height: 32px;
            line-height: 32px;
            font-size: 18px;
            color: #11192d;
            font-weight: 700;
        }
        .pick-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            background-color: #fff;
            .item {
                background-color: #fff;
                border-radius: 12px 12px 0 0;
                cursor: pointer;
                float: left;
                height: 368px;
                margin: 0 0 16px 16px;
                position: relative;
                transition: all 0.5s;
                width: 260px;
                img {
                    border-radius: 8px;
                    height: 240px;
                    overflow: hidden;
                    width: 240px;
                }
                .info {
                    margin-top: 8px;
                    margin-bottom: 8px;
                    font-size: 16px;
                    font-weight: 600;
                    line-height: 24px;
                    color: #11192d;
                }
                .price-wrapper {
                    display: flex;
                    align-items: center;
                    .price-unit {
                        color: #ff6200;
                        font-size: 16px;
                        line-height: 16px;
                        margin-right: 2px;
                    }
                    .price-value {
                        color: #ff6200;
                        font-family: Alibaba Sans\102, sans-serif;
                        font-size: 24px;
                        font-weight: 700;
                        line-height: 36px;
                    }
                    .price-sale {
                        color: #50607a;
                        font-size: 14px;
                        line-height: 16px;
                        margin-left: 8px;
                    }
                }
            }
        }

    }
}
.clearfix ::after{
    content: "";
    display: block;
    height: 0;
    clear: both;
    visibility: hidden;
}
</style>
