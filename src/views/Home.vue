<template>
  <div class="home">
    <div class="card">
      <div class="content">{{ text }}</div>

      <div class="cover"></div>
    </div>
    <Button @click="handleNextPage">下一页</Button>
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: "Home",
  data() {
    return {
      text: `　經名：析疑指迷論。元代神峰逍遙大師牛道淳撰。一卷。底本出處：《正統道藏》洞真部衆街類。

　　析疑指迷論序

　　神峰逍遙大師，出示高論二編，名曰《析疑指迷》。清談不吝於胸懷，奧妙發揮於翰墨，平生所養，於玆見矣。幸緣一覽，俾予泠泠然獨立於通衢，不知四肢之有無，則可以墻塹玄門，梯航後學者。大德戊戌仲春朔，汝南重玄子劉道真謹跋。

　　前火傳後火，薪異而焰同。今聖嗣古聖，時殊而道一。故宜乎馬、譚、劉、丘已來，演玄風敷妙化之真人，繼繼而出也。神峰逍遙先生牛君練師，新出奇論二卷。目曰《析疑指迷》，屬余以文開卷，一閱不覺身世兩忘，若馭清飆而遊乎碧落矣。其誘人也，循循然有條而不紊，使人惑志頓消而朗徹。其進人也，端語一發，使人浩然長往而不留。其言簡，其理微，其示教也深，其用心也切，此可謂火傳而聖繼者也。門人恐其微言將沒，裒而錄之，以禆後進。其弘師之道如是，此亦可謂用心之厚者焉。時大德三年中秋前三日，靜安沖漠道人王道亨書。

　　神峰逍遙子閑居幽室，倚軒塊坐，隱几忘懷。適有悟真子李志恒，從座而起，恭然而立，携牋作禮，拜而謂曰：敢問全真妙理，至道精微，性命之義，修行次序？願師演而析疑矣。逍遙子答曰：夫至道精微，無形無名，難演難言，非容取捨而可得也。故心困焉而不能知，口辟焉而不能辭，在人虛府自悟耳。其人叩之不已，志之愈誠，由是不得已而應命。輒述是論，名曰《析疑指迷》，庶資初學之漸悟耳。時元貞二年孟春上元日題。`,
      right: 0,
    };
  },
  created() {},
  methods: {
    handleNextPage() {
      console.log("下一页");
    },
  },
};
</script>
<style scoped>
.home {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: 100vh;
}
.card {
  width: 460px;
  height: 690px;
  border-radius: 5px;
  box-shadow: 0px 0px 5px rgba(0, 0, 0, 0.5);
  white-space: pre-wrap;
  writing-mode: vertical-rl;
  padding: 19px;
  font-size: 19px;
  line-height: 40px;
  overflow: hidden;
  /* text-decoration: underline; */
  position: relative;
}
.content {
  position: relative;
}
.cover {
  box-sizing: border-box;
  background-color: rgba(0, 0, 0, 0.1);
  position: absolute;
  left: 0;
  right: 0;
  top: 0;
  bottom: 0;
}
</style>
