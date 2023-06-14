# Проект по АнДану
### Выполнили Сафина Алия и Петрова Марьяна.

Для анализа мы взяли готовый датасет "Spotify and Youtube". Он сожержит информацию по популярным трекам в Spotify и их клипам на Youtube. Датасет был взят с сайта - https://www.kaggle.com/datasets/salvatorerastelli/spotify-and-youtube.

Сам датасет можно найти тут:
 https://drive.google.com/file/d/192nYZKPER6nxo15LaIIqDqoE8cxt8GRq/view?usp=share_link

Основная задача - проанализировать треки с точки зрения их характеристик, таких как танцевальность, громкость, энергичность и тд. 

Сначала мы просто ищем зависимости между признаками, пытаемся их устранить или используем в своих целях (например, для создания новых более репрезентативных характеристик). Далее на основе обработанных данных мы строим гипотезы и проверяем их.

1. Признак "Loud_and_Energetic" не влияет на кол-во просмотров. Мат. ожидания кол-ва просмотров трека с низким значением признака и с высоким равны.
2. Признак "Non_Instrumental_Loudness" имеет нормальное распределение.
3. Чем выше значение признака "Danceability", тем больше эмоций трек вызывает у пользователей и тем больше доля лайков к общему числу просмотров.

Следующий шаг - моделирование. Нас интересует признак Danceability и мы хотим посмотреть, можно ли его предсказать по таким параметрам, как Loudness & Energy, Non_Instrumental_Loudness, Not_Acoustic, Valence. 
