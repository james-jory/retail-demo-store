<template>
  <ArticleLayout>
    <template #heading>User Personalization</template>

    <template #recipe>
      Amazon Personalize Recipe:
      <a
        href="https://docs.aws.amazon.com/personalize/latest/dg/native-recipe-user-personalization-v2.html"
        target="_blank"
        rel="noreferrer noopener"
        >User-Personalization-v2</a
      >
    </template>

    <p>
      Product and content recommendations tailored to a user's profile and habits are more likely to drive higher
      conversion. Amazon Personalize helps tailor recommendations to users behavior, preferences, and history, boosting
      their engagement and satisfaction in real-time, instead of providing a uniform experience. User personalization
      also handles the “cold-start” challenge where limited or no historical information is known about an item or user.
      User personalization in Amazon Personalize balances recommending fresh items with the most relevant based on a
      user's unique preferences and behaviors.
    </p>

    <p>
      User personalization is implemented in the “Inspired by your shopping trends” section on the homepage. Try using different
      shoppers to experience the difference in personalized product recommendations offered.
    </p>

    <p>If you're not signed in, popular products will be initially displayed instead on the homepage. After clicking on a few products, those 
      interactions will be sent to Personalize to learn your interests. Then the application will automatically switch from displaying 
      popular products to recommendations using a ML model trained with the User-Personalization-v2 recipe.</p>

    <p>The User-Personalization-v2 recipe uses a transformer-based architecture to train a model that learns context and tracks relationships 
      and patterns in your data. Transformers are a type of neural network architecture that transforms or changes an input sequence into an 
      output sequence. For Amazon Personalize, the input sequence is a user's item interaction history in your data. The output sequence is 
      their personalized recommendations.</p>
  </ArticleLayout>
</template>

<script>
import ArticleLayout from '../ArticleLayout.vue';

export default {
  name: 'UserPersonalization',
  components: { ArticleLayout },
};
</script>

