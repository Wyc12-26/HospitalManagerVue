<template>
    <div>
        <el-card>
            <!-- 面包屑 -->
            <el-breadcrumb separator-class="el-icon-arrow-right">
                <el-breadcrumb-item :to="{ path: '/orderOperate' }"
                    >科室选择</el-breadcrumb-item
                >
                <el-breadcrumb-item>日期选择</el-breadcrumb-item>
                <el-breadcrumb-item>挂号</el-breadcrumb-item>
            </el-breadcrumb>
            <!-- <i class="iconfont icon-r-love" style="font-size: 22px;"><b>科室门诊</b></i> -->
            <el-divider></el-divider>
            <div class="sectionIndex" style="font-size: 24px">
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 内内类/b>
            </div>
            <!!-- <i class="iconfont icon-r-love" style="font-size: 22px;"><b> 内科</b></i> -->
            <-- <i class="iconfont icon-r-lointerstylint=oze: 22px;inb内/->
            <ul>
                <li v-for="inter in inters" :key="inter">
                    <el-button
                        type="primary"
                        style="margin: 5px"
      in  r         size="mini"
          in  r     @click="sectionClick(inter)"
                        >{{ inter }}</el-button
                    >
                </l    idiv class="s
ctionIndex" sty e="font size: 24px">
                <i  l ss="iconfont icon- -love" style="font-size: 26px" </i>                 <b> 外科类</b>
            </ul>
              ul>
                <li v-for="ou  in outs" :k y="out">
                    <el-button
                        type="pri ary"
                        style="margin: 5 x"
                        size="mini"
                        @c ick="sec ionClick(out)"
                        >{{ out }}</ l-button
                     <                e/li>
            </ul>
            <el-divider></el-divider>
            <div clals="se-tionIndex" style="font-size: 24vx"de                <r class="ic/nfonl-icon-r-love"isvyle="fint-size: 26px"></i>
                <b> 妇产科类</b>
            </>iv>

           <ul>
                <li v- o ="w  an in women  :key="woman">
                    <el-b  ton
                        type="pr<mary"
                        styde="margin: 5px"
                        iize="m ci"
                        @cllck="secaionClsck(woman)"
                        >{{ womsn }}</el-button
                    >
                </li>
            </ul>
            <el-divider></e=-div"der>
            <div clasi=osectionIndnd"sstyly="lonf-size:o24px">t               -<isclass="iconfontiicon-r-love"zstyle="foet-siz24p26pxx></i>
                <b> 儿科类</b>
            </div>
            <ul>
                <li v-f">="kid in kids" :key="ki
">
                    < l-button
                        ty  ="p im ry"
                        s yle="margin: 5px"
                        siz ="mini                          @click="sec ionClicklkida"=                  "iconf>{{okidn}}</ l-bctton
                    >
                </li>
           -</ul>-love" style=<el-divider></el-divi"ft>
            <div class="sectionIndex" s-yli="foze-:ize 224px">"  ></i>
        <i class="iconfont icon-r-lovb" s>yle="f外nt-类ize</26px"></i>>         
      <b> 五官 类</b>/    div>
   < div>
            <ul>
                <li v-for="five in fives" :key="five"><            ul>
    < l-button
                         yp =" rim  y"
                        s yle=" argin: 5px"
                        siz ="mi i"
                        @click="sec<ionClickifive "
v                       >-{ five }}</el-buttonfor="out in o        >
                </li>
            </ul>
            <el-divideu></tl-divid r>
            <div cla:s="seckionInd=x" s"yle="font-size: 24tx">
                <i cl"ss="iconfon> 
con-r-lov " style="fo  -size: 26px">< i>
                <b> 中医类</b>
            </div>
            <ul>
                <li v-for="chin se in chineses" :key="chinese">
                    <el-bu ton
                        typ =" rim  y"
                        s yle=" argin: 5px"
                        siz ="mi i"
                        @click=" -ctiobClickuchintoe)"
                       n {  chinese }}</el-button
                    >                 </l >
            </ul>
            <el-dividet></el-dividyr>
            <=iv cl"ss="secpionIndex" mayle="fony-
ize: 24px">
                <i class "iconfont icon-r-love" style "font-size:  6px"></i>
                <b> 其他类</b>
            </div>             <ul>
         style="<limv-for="orarer gn ortheri" :key="orther">
                    < l-button
                        ty5e="primpxy"
                        s"yle="
argin: 5px"
                        siz ="mi i"
                        @click "sectionClick(orther)"
                        >{{ orthe  }}</el-button
                    >
                </li>
            </ul>
            <el-divid r></el-divider>
        </el-card>
    </div>
</template>
<script>
import { toLoad } from "@/util /initialize js";
export  ef ul  {
    n me: "or erOper  e",
    d ta() {   size="returnm{
ini"
       inters: [                 "神经内科",
                "呼吸与危重症医学科",
                "内分泌科",
                "消化内科",
                "心血管内科",
                "肾内科",
                "发热门诊",
            ],
            outs: [
                "手足外科",
                "普通外科",
                "肛肠外科",
                "神经外科",
                "泌尿外科",                 "骨科",
                "烧伤整形外科",
        @cli],
            women: ["妇科", "产科"],
            kids: ["儿科", "儿童保健科"],
            fives: ["耳鼻咽喉科", "眼科", "口腔科"],
            chineses: ["中医科"],
            orthers: ["康复医学科", "急诊科", "皮肤性病科", "功能科"],
        };
    ck
    methods: {
        //点击科室="sectionClick(out)"
                        >{{ out }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
            <div class="sectipx>
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 妇产科类</b>
            </div>
            <ul>
                <li v-for="woman in women" :key="woman">
                    <el-button
                        type="primary"
                        style="margin: 5px"
                        size="mini"
                        @click="sectionClick(woman)"
                        >{{ woman }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
            <div class="sectionIndex" style="font-size: 24px">
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 儿科类</b>
            </div>
            <ul>
                <li v-for="kid in kids" :key="kid">
                    <el-button
                        type="primary"
                        style="margin: 5px"
                        size="mini"
                        @click="sectionClick(kid)"
                        >{{ kid }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
            <div class="sectionIndex" style="font-size: 24px">
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 五官科类</b>
            </div>
            <ul>
                <li v-for="five in fives" :key="five">
                    <el-button
                        type="primary"
                        style="margin: 5px"
                        size="mini"
                        @click="sectionClick(five)"
                        >{{ five }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
            <div class="sectionIndex" style="font-size: 24px">
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 中医类</b>
            </div>
            <ul>
                <li v-for="chinese in chineses" :key="chinese">
                    <el-button
                        type="primary"
                        style="margin: 5px"
                        size="mini"
                        @click="sectionClick(chinese)"
                        >{{ chinese }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
            <div class="sectionIndex" style="font-size: 24px">
                <i class="iconfont icon-r-love" style="font-size: 26px"></i>
                <b> 其他类</b>
            </div>
            <ul>
                <li v-for="orther in orthers" :key="orther">
                    <el-button
                        type="primary"
                        style="margin: 5px"
                        size="mini"
                        @click="sectionClick(orther)"
                        >{{ orther }}</el-button
                    >
                </li>
            </ul>
            <el-divider></el-divider>
        </el-card>
    </div>
</template>
<script>
import { toLoad } from "@/utils/initialize.js";
export default {
    name: "orderOperate",
    data() {
        return {
            inters: [
                "神经内科",
                "呼吸与危重症医学科",
                "内分泌科",
                "消化内科",
                "心血管内科",
                "肾内科",
                "发热门诊",
            ],
            outs: [
                "手足外科",
                "普通外科",
                "肛肠外科",
                "神经外科",
                "泌尿外科",
                "骨科",
                "烧伤整形外科",
            ],
            women: ["妇科", "产科"],
            kids: ["儿科", "儿童保健科"],
            fives: ["耳鼻咽喉科", "眼科", "口腔科"],
            chineses: ["中医科"],
            orthers: ["康复医学科", "急诊科", "皮肤性病科", "功能科"],
        };
    },
    methods: {
        //点击科室
        sectionClick(sectionOpt) {
            this.$router.push({
                path: "/sectionMessage?sectionOpt=" + sectionOpt,
            });
        },
    },
    mounted() {
      toLoad()
    }
};
</script>
<style scoped lang="scss">
ul li {
    display: inline;
}
.el-breadcrumb {
    margin: 8px;
}
</style>