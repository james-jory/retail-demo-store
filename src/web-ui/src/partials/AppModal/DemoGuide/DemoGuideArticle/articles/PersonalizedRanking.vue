<template>
  <ArticleLayout>
    <template #heading>Personalized Ranking</template>

    <template #recipe>
      Amazon Personalize Recipe:
      <a
        href="https://docs.aws.amazon.com/personalize/latest/dg/native-recipe-personalized-ranking-v2.html"
        target="_blank"
        rel="noreferrer noopener"
        >Personalized-Ranking-v2</a
      >
    </template>

    <p>
      Regularly your business priorities require you to promote specific content or products, such as trending news, a
      hit new TV show, seasonal merchandise, or a time bound promotional offer. Whether the source is a person, business
      rules around product lifecycle management, or a line of code, Amazon Personalize enables you to re-rank a subset of your
      product catalog to achieve your business priorities and best customer experience.
    </p>

    <p>
      The Personalized-Ranking-v2 recipe uses the same HRNN algorithm underneath User-Personalization-v2 but takes in a user AND a collection of items. This
      will then look at the collection of items and rank them in order of most relevant to least for the user. This is
      great for promoting a pre-selected collection of items and knowing what is best to promote for a
      particular user.
    </p>

    <p>
      You can see the personalized ranking use-case on the on the “Featured” products view on the homepage. The products are re-ranked
      based on the fictitious shopper's historical and real-time activity. The personalized-ranking model is also used to re-rank 
      search results.
    </p>

    <p>The Personalized-Ranking-v2 recipe uses a transformer-based architecture to train a model that learns context and tracks relationships 
      and patterns in your data. Transformers are a type of neural network architecture that transforms or changes an input sequence into an 
      output sequence. For Amazon Personalize, the input sequence is a user's item interaction history in your data. The output sequence is 
      their personalized recommendations.</p>
  </ArticleLayout>
</template>

<script>
import ArticleLayout from '../ArticleLayout.vue';

export default {
  name: 'PersonalizedRanking',
  components: { ArticleLayout },
};
</script>
