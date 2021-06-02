<template>
    <div>
        <section class="hero is-link">
            <div class="hero-body">
                <p class="title">
                    <i class="fas fa-glass-martini-alt"></i> 피아노의
                    <i class="fas fa-glass-cheers"></i> 모든것
                </p>
                <p class="subtitle">
                    피아노의 색상을 선택해주세요
                </p>
            </div>
        </section>
        <section class="columns">
            <div class="column">
                <table class="table">
                    <thead>
                        <tr>
                            <th>번호</th>
                            <th>색깔</th>
                        </tr>
                    </thead>
                    <tbody>
                        <template v-for = "pos in tablepiano_color1.length"> 
                            <tr :key= "pos">
                                <td>{{pos}}</td>
                                <td>{{tablepiano_color1[pos - 1]}}</td>
                            </tr>
                        </template>
                    </tbody>
                </table>
            </div>
            <div class="column">

            </div>
        </section>
    </div>
</template>
<script>
	import piano_color1 from "/~assets/colors1.json";
	import piano_color2 from "/~assets/colors2.json";
	export default{
		data(){
			return { tablepiano_color1:  piano_color1.colors,
                    tablepiano_color2:  piano_color2.colors
			};
		}
	};
</script>