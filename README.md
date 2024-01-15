# Association Rule Learning 
## Study of "What goes with what!"
 - Association rule mining finds interesting associations and relationship amoung large sets of data items. this rule shows how frequent a itemset occurs in a transaction. 
 - Market Basket Analysis is one of the key technique used by retailers to increase purchasing patterns. it involves analyzing large data sets such as purchase history to reveal product groupings as well as 
  products that are likely to be purchased together.
### Rule From 
### Antecedent → Consequent [ Support, Confidence]
  • An antecedent is an item found withing the data and a Consequent is an item found in combination with the antecedent (an antecedent is 1st purchase and depending on uour 1st purchase what you buy bext is Consequent)
  Eg. If you buy Bred then probability of you buying Butter is high but if you buy Butter 1st then there is very low probability of you buying Bred as your next purchase depending on your 1st purchase.
  
### Support
- Support indicates how frequently an item or item-set appears in the dataset or transaction.

### Confidence
- Confidence indicates how frequently a rule is found to be true.

### Lift
- Lift (A →B) indicates the rise in probability of occurrence of B when A has already occurred. 
 
### For a rule, if {A} →{B} has high confidence, then it indicates that B is more likely to occur with A.
### For rule {A} →{B}

By computing support, we know whether the rule is important or not.

By computing confidence, we can able to know that how likely A and B will occur together.

Although these computations are important, they do not give us any idea on what extent the occurrence of one item (say A) or item-set increase the occurrence of the other item (say B) or item-set.

So, we have to calculate lift, to know how the antecedent (independent item or data) and consequent (dependent data) are related to one another.

For a rule: {Antecedent} →{Consequent}

If lift = 1, then the possibility of occurrence of Antecedent and Consequent are not dependent on each other.

If lift < 1, then the occurrence of Antecedent has negative effect on occurrence on Consequent and Antecedent has positive effect on occurrence on Consequent.

If lift > 1, then that the two occurrences are dependent on each other, and these rules are very useful in identifying the consequent in final cases. It also helps us know that to what extent the occurrences are dependent on each other.

There are different algorithms which are used to implement association rule learning technique.
## Apriori Algorithm
Apriori algorithm is a standard algorithm in Association Rule Learning in Data mining. It is used for drawing familiar item sets and their relevant association rules. It is designed to perform on a database.

It is very important for effective Market Basket Analysis and it helps in understanding the businessman that which items customers will buy together. It has also been used in healthcare field for the discovery of adverse drug reactions. It generates association rules that shows what are all combinations of medications and patient characteristics which will help in effective drug delivering.

## Eclat Algorithm
Eclat algorithm is a type of Association rule learning algorithm. It can be applied to achieve itemset mining. Itemset mining helps us to obtain periodic patterns in data. For example, if a consumer buys shoes, he would also buy socks. The main purpose of this algorithm is to use set intersections to calculate the support of a candidate itemset avoiding the generation of subsets that does not exist in the prefix tree.

Eclat algorithm performs a depth-first search to count the number of columns. Therefore, Eclat algorithm performs faster than the Apriori algorithm.

## F-P Growth Algorithm
The Full form of F-P Growth algorithm is Frequent Pattern growth Algorithm. The FP Growth classification is used only with databases but not with streams. Apriori algorithm needs n+1 number of scan if a database is utilized, here n is the length of the longest model. We can decrease number of scans of complete database by two by using F-P growth Algorithm.
