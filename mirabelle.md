# Mirabelle: Revolutionizing Podcast Advertising with Multi-Lingual, Context-Aware Ad Insertion

# **Executive Summary**

Podcast advertising is a burgeoning market, projected to exceed $2.5 billion by 2024 [1](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-1). However, significant challenges remain in delivering relevant and engaging ads to an increasingly diverse and mobile listener base. This white paper explores these challenges, particularly language mismatch and irrelevant targeting, and introduces **Mirabelle**, a dynamic ad insertion solution designed to enhance ad relevance and unlock new opportunities for advertisers and podcast platforms.

# **The Problem**

## **Current State of Podcast Advertising**

Podcast advertising is experiencing substantial growth, with U.S. ad revenues reaching $1.9 billion in 2023, a 5% increase from the previous year [2](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-2). Despite this growth, podcast advertising represents only 0.2% of total advertising budgets, highlighting significant potential for expansion [3](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-3). However, this growth is threatened by ineffective ad targeting strategies.

## **Key Issues**

1. **Language Mismatch**: Listeners often encounter ads in languages they do not understand, especially when traveling or listening to podcasts in non-native languages. Consider the experience of an English speaker in Croatia hearing Croatian-language ads – a wasted impression and a frustrating experience for the listener.

2. **Irrelevant Targeting**: Current geolocation-based targeting fails to account for travelers or multilingual listeners, leading to irrelevant and ineffective ads.

3. **Ad Repetition**: Listeners frequently experience the same ads repeatedly, leading to "ad fatigue" and decreased engagement.

4. **Limited Advertiser Pool**: Many podcasts struggle with a lack of diverse advertisers, resulting in repetitive and unengaging ad content.

## **Impact on Stakeholders**

* **Listeners**: Experience confusion and frustration with irrelevant or incomprehensible ads, leading to ad-skipping and disengagement. A recent study showed that over 60% of listeners skip ads that are not relevant to them [4](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-4).

* **Advertisers**: Waste ad spend on poorly targeted campaigns, resulting in lower conversion rates and diminished ROI. This reluctance is costing advertisers money.

* **Podcast Platforms**: Risk undermining credibility and user trust due to misaligned ad serving. Also leading to opportunity for increased advertising revenue through better ROI. Some major platforms, like iHeartRadio and Wondery, exacerbate the problem by repeatedly playing ads for their own shows, creating a frustrating experience for listeners who are already familiar with the content [5](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-5).

# **Mirabelle: A Multi-Lingual, Context-Aware Solution**

To address these challenges, we introduce **Mirabelle**, a dynamic ad insertion solution that suggests prioritizing relevance by leveraging multiple factors:

1. **Podcast Language**

2. **Device Language Settings**

3. **Geolocation**

Mirabelle aims to deliver more targeted and engaging ads to listeners, creating a better experience for both listeners and advertisers.

## **Implementation Strategy**

Mirabelle utilizes a decision tree to select the most relevant ad based on the available information:

1. **Podcast Language Only**: Serve universal ads in the podcast’s language (e.g., English podcast \= English language ad for Google Search, YouTube Music, gaming apps).

2. **Podcast Language \+ Device Language**:

   * If matching: Serve universal ads in that language.

   * If different: Offer bilingual ads or ads targeting language learners (e.g., language learning apps, flight rewards programs).

3. **Podcast Language \+ Geolocation**:

   * If matching: Deliver targeted local ads.

   * If different: Serve ads for local services in the podcast language (e.g., French cultural events in Chicago for French podcast listeners).

4. **All Factors Different**: Target ads for travelers or international services.

**Example Scenario:**

Consider an English-speaking expat living in Berlin listening to an English-language podcast. With Mirabelle, this listener would receive ads tailored to their specific situation – ads for English-language services in Berlin, rather than generic German ads that are irrelevant and frustrating.

## **Technical Implementation**

Mirabelle leverages existing API functionalities for ad serving, language detection, and geolocation:

1. **Ad Serving**: Mirabelle leverages dynamic ad insertion using APIs such as Google Ad Manager API or AdMob API. These APIs enable real-time ad selection and insertion based on contextual data.

2. **Language Detection**: To retrieve device language settings, Mirabelle uses the `Locale.getDefault()` method in Java/Android.

3. **Geolocation**: Location services and APIs (such as Google Maps APIs, CoreLocation for iOS, or geocoder APIs) are used for location detection.

## **Benefits**

* **Improved Ad Relevance**: By delivering more targeted ads, Mirabelle significantly improves ad relevance for listeners. This is especially critical considering that 53% of listeners are likely to purchase from brands advertised on podcasts [6](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fn-6), a figure that can be significantly increased by enhancing ad relevance.

* **Increased Engagement**: Relevant ads lead to higher engagement rates and lower ad-skipping rates. Listeners are more receptive to ads that are tailored to their interests and needs. This increased level of ad engagement increases the ROI.

* **Expanded Advertiser Base**: Mirabelle opens up opportunities to attract a more diverse range of advertisers, including local businesses and international brands targeting specific listener segments. This expanded pool will decrease listener fatigue around repetition and entice new people to test podcast ads with their media spend.

* **Enhanced User Experience**: By reducing irrelevant ads and ad repetition, Mirabelle enhances the overall podcast listening experience.

# **Addressing Key Challenges**

## **Monetization & ROI**

Mirabelle directly addresses monetization challenges by reducing ad waste and improving listener engagement. By providing more relevant ads, Mirabelle suggests increasing the value of ad inventory, leading to higher CPMs (Cost Per Mille) and attracting more advertisers.

## **Competitive Landscape**

While some platforms utilize dynamic ad insertion, Mirabelle stands out with its multi-lingual, context-aware approach. It goes beyond simple geolocation targeting to consider both podcast and device language, creating a more personalized and effective ad experience. Major platforms such as iHeartRadio and Wondery, may offer a poor user experience.

## **Partnerships & Integrations**

Mirabelle could be implemented in partnership with podcast platforms and indie podcasters to integrate Mirabelle into a broader ecosystem.

## **Future Trends**

Mirabelle aligns with future trends in podcasting and advertising, particularly the use of AI for ad targeting and efficiency. AI-driven language detection and contextual ad delivery can further enhance Mirabelle’s capabilities, ensuring that ads are always relevant and engaging.

## **Data Privacy**

Mirabelle respects user privacy by primarily relying on podcast language and user-provided information. By not collecting or storing unnecessary personal data, Mirabelle ensures compliance with data privacy regulations like GDPR and CCPA. Mirabelle puts power into user hands by allowing them to specify if geolocation or device setting should be used in ad serving. We are only using available data.

## **Scale and Implementation**

Technical infrastructure (ad servers, language detection) and real-world testing are key hurdles. However, by leveraging existing API functionalities and focusing on a phased implementation, these challenges can be effectively addressed.

# **Conclusion**

By addressing the language and context issues in podcast advertising, Mirabelle unlocks the full potential of this rapidly growing medium. Mirabelle not only benefits listeners with a more engaging experience, but also creates new opportunities for advertisers and platforms alike.

# **Contact to Learn More** 

We invite collaboration from podcast platforms, advertisers, and ad tech companies to refine and implement Mirabelle. Your insights and feedback are crucial in shaping the future of podcast advertising.

For further discussion or to contribute to this initiative, please comment, email [hello@mandyfifi.com](mailto:hello@mandyfifi.com) or reach out via [LinkedIn](https://www.linkedin.com/in/mandyfiona/)

## **Footnotes**

1. [https://www.iab.com/wp-content/uploads/2024/05/IAB\_US\_Podcast\_Advertising\_Revenue\_Study\_FY2023\_May\_2024.pdf](https://www.iab.com/wp-content/uploads/2024/05/IAB_US_Podcast_Advertising_Revenue_Study_FY2023_May_2024.pdf) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-1)

2. [https://www.incrmntal.com/resources/podcast-advertising](https://www.incrmntal.com/resources/podcast-advertising) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-2)

3. [https://www.spiralytics.com/blog/podcast-marketing-advertising-statistics/](https://www.spiralytics.com/blog/podcast-marketing-advertising-statistics/) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-3)

4. [https://advertise.acast.com/news-and-insights/why-podcast-advertising-is-effective-benefits-and-statistics-for-2023](https://advertise.acast.com/news-and-insights/why-podcast-advertising-is-effective-benefits-and-statistics-for-2023) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-4)

5. [https://www.iab.com/insights/us-podcast-advertising-revenue-study-2024/](https://www.iab.com/insights/us-podcast-advertising-revenue-study-2024/) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-5)

6. [https://www.cohostpodcasting.com/resources/podcast-statistics-marketers-should-know](https://www.cohostpodcasting.com/resources/podcast-statistics-marketers-should-know) [↩](https://www.perplexity.ai/search/problem-podcast-ads-there-are-WOSSJyphQyaagbt4BrQKAg#user-content-fnref-6)

