<template>
    <div class="pay">
        <el-row>
           <div style="width: 1200px;height: 400px">
                <div style="text-align: left;padding: 100px 10px;padding-bottom: 0;position: relative;">
                    <img src="../../../assets/shopcart/图层46拷贝2.png" alt="" style="float: left">
                    <div style="width: 2px;height: 20px;background:#ccc;border-radius: 10px;float: left;margin-top: 5px;margin-left: 5px"></div>
                    <div style="float: left;margin-left: 10px">
                        <p style="font-weight: 600;font-size: 16px">订单提示</p>
                        <p style="font-size:9px;color: #9f9f9f">ORDER TIPS</p>
                    </div>
                    <div style="width: 67px;height:67px;background-color: #5ed5e0;color: white;opacity: 0.9;border-radius: 100%;text-align:center;font-size:30px;line-height:70px;position:absolute;left: 95px;top:65px;z-index: -1"><span style="opacity: 0.7">01</span></div>
                </div>

               <div class="ord-l">
                   <div style="margin-bottom:35px ">
                       <p>～ 订单提交成功啦，赶紧付款吧</p>
                   </div>
                   <div>
                      <div style="float: left">～</div>
                       <div class="dsq" >
                            <div >   30<span>min</span></div>
                           <div>   00 <span>s</span></div>
                           <div>   00 <span>ms</span></div>
                       </div> 后将自动取消订单
                   </div>
                   <div class="ord-text">
                       <span>～ 订单号是：</span>
                       <span>2019042814458299</span>
                       <span>～ 支付金额：</span>
                       <span>3146.00</span>
                       <span>RMB</span>
                   </div>
               </div>
               <div class="ord-r">
                   <img src="../../../assets/shopcart/图层64.png" alt="">
               </div>

           </div>
        </el-row>
        <el-row>
            <div style="width: 1200px;height: 400px">
                <div style="text-align: left;padding: 100px 10px;padding-bottom: 0;position: relative;">
                    <img src="../../../assets/shopcart/图层46拷贝2.png" alt="" style="float: left">
                    <div style="width: 2px;height: 20px;background:#ccc;border-radius: 10px;float: left;margin-top: 5px;margin-left: 5px"></div>
                    <div style="float: left;margin-left: 10px">
                        <p style="font-weight: 600;font-size: 16px">支付方式</p>
                        <p style="font-size:9px;color: #9f9f9f">PAYMENT METHOD</p>
                    </div>
                    <div style="width: 67px;height:67px;background-color: #5ed5e0;color: white;opacity: 0.9;border-radius: 100%;text-align:center;font-size:30px;line-height:70px;position:absolute;left: 95px;top:65px;z-index: -1"><span style="opacity: 0.7">02</span></div>
                </div>
                <div style="margin-top: 50px">
                    <el-row>
                        <el-radio v-model="radio" label="1"  border  style="width: 570px;height: 70px;line-height: 45px;margin-top: 20px;background-color: #f6f6f6">快捷支付(点击第三方设备进行付款)</el-radio>
                        <el-radio  v-model="radio" label="2" border  style="width: 570px;height: 70px;line-height: 45px;margin-top: 20px ;background-color: #f6f6f6">扫码支付</el-radio>
                    </el-row>
                    <el-row  style="margin: 20px;text-align: left;margin-left: 50px">
                        <el-radio v-model="radio1" label="1"><img src="../../../assets/shopcart/图层65.png" alt=""></el-radio>
                        <el-radio v-model="radio1" label="2"><img src="../../../assets/shopcart/图层66.png" alt=""></el-radio>
                    </el-row>
                    <el-row>
                        <el-radio  v-model="radio" label="3" border  style="width: 1180px;height: 70px;line-height: 45px;margin-top: 20px ;background-color: #f6f6f6">网银支付</el-radio>
                    </el-row>

                </div>

            </div>
        </el-row>
    </div>
</template>
<style scoped>
    .ord-l{
        float: left;
        margin-top: 60px;
        text-align: left;
         font-size:16px ;
        color:#666666 ;
        line-height: 35px;
    }
    .ord-r{
        float: right;
        margin-top: 30px;
        margin-right: 100px;
    }
    .dsq{
        width: 260px;
        height: 40px;
        border: 1px solid #e5e5e5;
        float: left;
        margin-right: 25px;
        text-align: center;
        line-height: 38px;
    }
    .dsq > div{
        float: left;
        width: 83px;
        border-right:2px solid #ffdede ;
        font-size: 20px;
        font-weight: 600;
        color: red;
    }
    .dsq :nth-child(3){
        border-right: none;
    }
    .dsq>div>span{
        font-size: 10px;
        color: black;
    }
    .ord-text{
        margin-top: 28px;

    }
    .ord-text>span{
        font-size:16px ;
        color:#666666 ;
    }
    .ord-text>span:nth-child(2){
        font-size: 28px;
        font-weight: 600;
        color: black;
        margin-right: 30px;
        line-height: 45px;
    }
     .ord-text>span:nth-child(4){
         font-size: 28px;
        font-weight: 600;
        color: black;
        margin-right: 5px;
        line-height: 45px;
     }
    .ord-text>span:nth-child(5){
        font-size: 10px;

    }

</style>
<script>
export default {
    name:'shopping',
     data () {
      return {
        radio: '1',
          radio1:'1',

      };
    },
    // created(){
    //     this.Time()
    // },
    // Time(){
    //     setInterval(()=>{let now = new Date()})
    //     let future = new Date("2019-11-8 8:00:45")
    //     let offset = Math.floor((future.getTime()-now.getTime())/1000) //天
    //     let hourNum = Math.floor(offset/(60*60))
    //     this.hour=hourNum
    //     let minNum = Math.floor((offset)%(60*60)/60)
    //     this.minute = minNum
    //     let secNum = Math.floor(offset%(60*60)%60)
    //     this.sec = secNum
    //     this.time['hour'] = this.hour
    //     this.time['minute'] = this.minute
    //     this.time['sec'] = this.sec
    // }
}
</script>