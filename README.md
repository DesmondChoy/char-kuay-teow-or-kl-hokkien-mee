# Using Computer Vision models to discern different noodle dishes

For the uninitiated, [**Char Kway Teow**](https://en.wikipedia.org/wiki/Char_kway_teow) ("CKT") and [**KL Hokkien Mee**](https://thewoksoflife.com/malaysian-hokkien-mee/#:~:text=What%20is%20%E2%80%9CKL%E2%80%9D%20Hokkien%20Mee,I%20would%20skip%20this%20recipe!) ("KLHM") are famous noodle dishes in their respective countries - CKT can be found primarily in Singapore, while there are several variants of Hokkien Mee found in Malaysia. I'm only interested in the variant found in Kuala Lumpur (KL).  
I've tasted them and they are both heavenly, although I'll attest that the latter is more sinful (more pork lard is used).  
They look similar (in my opinion) and I'm curious how well a Computer Vision model with some fine-tuning can accurately discern CKT vs KLHM.

This notebook is heavily inspired by Jeremy Howard's [kaggle notebook](https://www.kaggle.com/code/jhoward/is-it-a-bird-creating-a-model-from-your-own-data) and his amazing course - [Practical Deep Learning for Coders](https://course.fast.ai/Lessons/lesson1.html).


<div style="display: flex;">
    <figure style="margin: 5px;">
        <img src="https://images.lifestyleasia.com/wp-content/uploads/sites/6/2023/01/27180753/best-char-kway-teow-singapore-hawker-stalls-heritage-local-food-hawker-centre.jpg?" width="400">
        <figcaption>Char Kway Teow</figcaption>
    </figure>
    <figure style="margin: 5px;">
        <img src="https://1.bp.blogspot.com/-JYKSvvSuJP8/X7hlGoQsEzI/AAAAAAABCfk/OPk0_qFpU5E9spa_p33sqgA0gNXyqCngACLcBGAsYHQ/s2048/KL%2BHokkien%2Bmee.jpg" width="400">
        <figcaption>KL Hokkien Mee</figcaption>
    </figure>
</div>
