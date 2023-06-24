# NLP-hot
Материалы с выступлений по NLP


Настоящее время - это эпоха трансформеров (архитектура была придумана в 2017 году Google). С 2021 года активно развивается направление генеративных языковых моделей (decoder-only трансформеров) https://arxiv.org/abs/1706.03762

Появились языковые модели уже просто гигантских размеров (н-р, PALM от Google на 540 миллиардов параметров)
У больших моделей (свыше примерно 100 млрд параметров) наблюдается, так называемая, emergent ability, то есть способность выполнять задачи, на которые данная модель не была обучена

Большие языковые модели дорого дообучать, в связи с этим появилось новое направление prompt engeeniring, то есть разработка "правильных" затравок
В свою очередь, в prompt engineering также появляются новые интересные направления, например, Chain-of-Thought

Трансформеры - это основа базовых моделей, но чтобы сделать эти модели более "человечными" моделями-ассистентами требуется дообучение. Хорошо себя показала методика RLHF. В настоящее время перспективно выглядит новый подход principle-driven self-ALIGN с минимальным вовлечением человека (так Dromedary удалось дообучить, используя менее чем 300 строк аннотаций, написанных людьми).

В качестве тренда можно выделить мультимодальность, пример, GPT-4

Среди SOTA генеративных моделей (decoder-only) можно выделить следующие из закрытых: GPT-4, ChatGPT (GPT-3,5); из open source: LLama, Alpaca, Stable Vicuna, Dromedary; от русскоязычных команд opensource: Yalm100B oт Яндекс, Saiga от команды Ильи Гусева; из корпоративных закрытых: GigaChat, YandexGPT. Также появляются модели-ассистенты под конкретные задачи, например, BloombergGPT. Среди моделей encoder-decoder: T5 и русскоязычные ruT5, FRED-T5. Среди encoder-only: семейство BERT.

Коротко некоторые проблемы в данной сфере: модели могут "галлюцинировать"; модели ограничены данными, на которых они обучались; все чаще встает вопрос воспроизводимости результатов научных статей (т.к. новые методы часто предназначены для гигантских закрытых моделей); вопрос открытости новых решений; вопрос регулирования данных разработок со стороны общества и др.

