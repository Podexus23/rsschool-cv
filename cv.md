# Anton Serovski

## Contacts

- Phone: +375 29 386 73 80
- E-mail: santon23@gmail.com
- Telegram: @usaty_podex
- GitHub: [Podexus23](https://github.com/Podexus23)

### About Myself:

Born with an insatiable curiosity and a desire to make a difference, I embarked on a journey of self-discovery and exploration from an early age. Through diligence and determination, I developed a passion for various mechanisms and the principles behind their functioning, which eventually led me to pursue higher education in the field of energy engineering.

What truly sets me apart is my ability to adapt to new challenges and draw lessons from every experience. I have a keen eye for detail, a collaborative spirit, and an innovative mindset, making me a valuable asset in any team.

Beyond the professional realm, I am passionate about fiction and comedy literature, music spanning different genres and generations, movies, and computer games.

As time progresses, I continue to seek new opportunities for growth and remain deeply passionate about technology, people, and the arts. My story is one of relentless pursuit of excellence and the belief that every challenge is an opportunity to learn and thrive.

---

### Skills:

- HTML
- CSS (SASS, BEM methodology)
- JavaScript (Fundamentals, OOP, FP, ES6+, DOM), TS
- Git, GitHub
- Module bundlers: WebPack, Parcel
- Node JS (Express)
- MongoDB (Mongoose)
- Figma (for Web Dev)
- VSCode
- AWS Cloud Quest: Cloud Practitioner

## Code Examples

interesting task from leetcode
Largest Rectangle in Histogram

```
function largestRectangleArea(heights) {
  let nextSmaller = new Array(heights.length).fill(heights.length);
  let previousSmaller = new Array(heights.length).fill(-1);
  let stack = [];
  for (let i = 0; i < heights.length; i++) {
    while (stack.length && heights[stack.at(-1)] > heights[i]) {
      let stackTop = stack.pop();
      nextSmaller[stackTop] = i;
    }
    if (stack.length) {
      previousSmaller[i] = stack.at(-1);
    }
    stack.push(i);
  }

  let maxArea = 0;
  for (let i = 0; i < heights.length; i++) {
    let currentHeight = heights[i];
    let width = nextSmaller[i] - previousSmaller[i] - 1;
    maxArea = Math.max(maxArea, currentHeight * width);
  }

  return maxArea;
}
```

## Work experience and examples

I working as System Administrator(network administrator and computer operator) at HC Gomel for almoust 2 years

- Here i worked with LeafLet and tried to use forms [Mapty](https://podexus23.github.io/10-Mapty/)
- Probably first work with API and kinda useful if you wanna make something to eat 😀 [Forkify](https://forkify11-23.netlify.app/#5ed6604591c37cdc054bcd09)

## Education:

- Gratuated at Sukhoi State Technical University of Gomel as Power Engeneer
- Studied JavaScript, Node JS on Udemy courses

### English

- [StreamLine Language School English test result:](https://test.str.by/login/index.php) A2
