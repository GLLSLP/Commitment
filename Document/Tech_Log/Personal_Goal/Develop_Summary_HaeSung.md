# ๊ฐ๋ฐ ์ผ์ง ๐ฑโ๐

> ํด์ฑ ๊ฐ๋ฐ ์ผ์ง 

<br>

## ์์๋ก๊ทธ์ธ ์ ๋ฆฌ ํ๊ฒ๋ค

[https://parkjihwan.tistory.com/9](https://parkjihwan.tistory.com/9)

ํ์ด์ค๋ถ,๊ตฌ๊ธ,์นด์นด์ค๋ก๊ทธ์ธ

[https://velog.io/@cloudlee711/vue-๊ตฌ๊ธ-๋ก๊ทธ์ธ-ํ๊ธฐ](https://velog.io/@cloudlee711/vue-%EA%B5%AC%EA%B8%80-%EB%A1%9C%EA%B7%B8%EC%9D%B8-%ED%9B%84%EA%B8%B0)

๊ตฌ๊ธ๋ก๊ทธ์ธ

## ํ์๊ฐ์๊ด๋ จ

import axiosํด์จ๋ค์์

axios.post('url', this.~~) ์ด๋ฐ์์ผ๋ก ๋ฐ๋ก์์ฑํ๋๋ฐ 

์ด๋ฐฉ๋ฒ์ด ์๋๋ผ ๋ค๋ฅธ ๋ฐฉ๋ฒ์ธ๊ฐ..? ์ฐ๋ฆฌ ํ๋ก์ ํธ์์๋ store๋๋์ด์ ธ์๊ณ  ๋  axios๊ฒฝ์ด

directory์์๋ account.js์์ ํ๋๊ฑฐ๊ฐ์๋ฐ ํท๊ฐ๋ฆฌ๋๊น ์ผ๋จ ์๋ฃ ์ฐพ์๋ด์ ์ฌ๊ธฐ๋ค๊ฐ ๋ฐ๋ก ์ ๋ฆฌํ๊ธฐ

```markdown
<!-- src/components/auth/signup.vue -->
......
<script>
  import axios from 'axios';
    
  export default {
    data () {
      return {
        email: '',
        age: null,
        password: '',
        confirmPassword: '',
        country: 'usa',
        hobbyInputs: [],
        terms: false
      }
    },
    methods: {
      ......
      onSubmit () {
        const formData = {
          email: this.email,
          age: this.age,
          password: this.password,
          confirmPassword: this.confirmPassword,
          country: this.country,
          hobbies: this.hobbyInputs.map(hobby => hobby.value),
          terms: this.terms
        }
        console.log(formData)
          
        axios.post('https://<project>.firebaseio.com/users.json', formData)
            .then(res => console.log(res))
            .catch(error => console.log(error))
      }
    }
  }
</script>
```

[https://velog.io/@jyongk/Vue.js-๋ก๊ทธ์ธํ์๊ฐ์-์์ Front-end](https://velog.io/@jyongk/Vue.js-%EB%A1%9C%EA%B7%B8%EC%9D%B8%ED%9A%8C%EC%9B%90%EA%B0%80%EC%9E%85-%EC%98%88%EC%A0%9CFront-end)

์ฐธ๊ณ  ์ฌ์ดํธ 1

## Infinite autoscrolling

[https://tympanus.net/codrops/2021/01/05/creating-an-infinite-auto-scrolling-gallery-using-webgl-with-ogl-and-glsl-shaders/](https://tympanus.net/codrops/2021/01/05/creating-an-infinite-auto-scrolling-gallery-using-webgl-with-ogl-and-glsl-shaders/)

webgl์ด๋ผ๋ ๊ฒ์ ์ด์ฉํด์ ์ผ๋จ ์ํตํ์ผ๋ก ๋ง๋ ๋ค์์ ๊ทธ์์ ์ฌ์ง์ ๋ฐฐ์นํ๊ณ  

๊ทธ๋ค์์ ์๋์ฐ์ฌ์ด์ฆ ๋ง์ถฐ์ ์กฐ์ ํ๊ณ  ๋ง์ฐ์ค๋ก ์คํฌ๋กค๋ค์ด์ํ ๋๋ง๋ค ์์์  ์กฐ์ ํด์ฃผ๋๋๋