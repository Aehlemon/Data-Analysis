### 🔎 Collaborative Filtering

- **Collaborative Filtering**: 아마존, 유투브, 넷플리스 등 정교한 추천 알고리즘의 일부로 활용 중이며 널리 사용됨
 - 같은 속성의 이용자들의 선호도 (좋고, 싫음)에 따라 제안을 주는 추천 학습기를 만드는 원리
 - 기본 전제로, 유사 군의 유저가 좋아하는 것을 좋아할 것이라는 가정을 바탕으로 만들어져서 이를테면
 - 로맨스를 좋아하는 사람들이 추천한 영화, 드라마를 로맨스를 자주 보는 사람이라면 노출되게 하는 것이다.

- Collaborative Filtering Questions:
 1. 유저 또는 아이템을 어떻게 유사한 그룹과 아닌 그룹으로 볼지?
 2. 어떻게 유사한 선호도를 갖는 유저가 남긴 평점을 바탕으로 어떤 평점을 줄지 예측할까?
 3. 예측한 또는 계산한 평점의 정확성은 어떻게 측정할 것인지?

- 1번 2번에 대한 내용을 중점적으로 보면 결국 "비슷한 속성의 유저와 아이템을 구분짓는 방법, 예를 들면 영화의 평점 등을 예측하려는 속성 값을
 - 구분짓는 방법에 의해 연결하여 예측/분류하는 알고리즘"으로서 `코사인 유사도`, 차원축소 기법 중 하나인 `Matrix factorization` (`SVD`), `K-NN` 등이 있다.

- 고객의 프로파일(성별, 연령, 관심사 등)으로 추천해주는 알고리즘을 찾고 있었는데...
> One important thing to keep in mind is that in an approach based purely on collaborative filtering, the similarity is not calculated using factors like the age of users, genre of the movie, or any other data about users or items. It is calculated only on the basis of the rating (explicit or implicit) a user gives to an item. For example, two users can be considered similar if they give the same ratings to ten movies despite there being a big difference in their age. by Abhinav Ajitsaria

- 위 내용에 따르면, 구매이력 정보나 연령에 따라 추천되는 것이 아니다! 프로젝트에 맞는 알고리즘을 추가적으로 서치해야겠다.

- [참고링크](https://realpython.com/build-recommendation-engine-collaborative-filtering/#model-based)



