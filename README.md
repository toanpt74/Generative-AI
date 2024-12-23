# Generative-AI
Một số tham khảo về Generative AI

https://github.com/microsoft/generative-ai-for-beginners/blob/main/01-introduction-to-genai/README.md






1. Giới thiệu về Generative AI
Generative AI là một mô hình trí tuệ nhân tạo có khả năng sinh ra dữ liệu mới từ dữ liệu quá khứ
Điều này có nghĩa là Generative AI không chỉ phân tích và dự đoán dựa trên dữ liệu hiện có mà còn có thể tạo ra nội dung mới hoàn toàn. 
Ví dụ, Generative AI có thể viết một bài văn, tạo ra một bức tranh, hay thậm chí sáng tác một bản nhạc mà không cần dựa trên bất kỳ nguồn dữ liệu cụ thể nào.

2. Tóm tắt lịch sử của các mô hình ngôn ngữ dựa trên mạng neural
Giai đoạn 1: Statistical Language Models (1990s)
1990 mô hình xử lý ngôn ngữ dựa trên xác suất ra đời (SLMs - Statistical Language Models) . Hai mô hình điển hình của phương pháp này là bigram và trigram. 
Các mô hình này chủ yếu dựa trên xác suất thống kê và tần suất xuất hiện của các từ trong câu.
tuy nhiên các mô hình này đều gặp khó khăn trong việc xử lý ngôn ngữ tự nhiên do tính đa ngữ nghĩa của ngôn ngữ.
Giai đoạn 2: Neural Language Models (2000s)
2000 mô hình mạng neuron nhân tạo đã dẫn tới một bước nhảy vọt trong các mô hình xử lý ngôn ngữ tự nhiên, các mô hình này xử lý ngôn ngữ tự nhiên không chỉ đơn giản dựa trên
các từ và tần xuất của chúng, mà chúng còn xem xét tới mối quan hệ của các từ trong câu.
Stage III: Pre-trained Language Models (2010s)
Khi mô hình xử lý ngôn ngữ tự nhiên dựa trên mạng neural ra đời, một loạt các mô hình pre-train được các hãng công nghệ lớn đưa ra nhằm giúp các nhà phát triển có thể tận dụng chúng
cho việc xử lý ngôn ngữ tự nhiên mà không cần phải phát triển từ đầu
Stage IV: Large Language Models (2020s)

Giai đoạn này các mô hình ngôn ngữ lơn ra đời, đây là các mô hình xử lý ngôn ngữ tự nhiên dựa trên mạng nơ ron và được huấn luyện trên các tập dữ liệu cực lớn giúp mô hình hiểu
tốt hơn về ngôn ngữ tự nhiên, ví dụ: GPT-2, Chat GPT-3, GPT-4, PaLM, Mistral,...


Gen AI và trí tuệ nhân tạo
+ AI: ............
+ Machine learning: .................
+ Deep learning: .........................
Generative AI: ...........................

3. Khái niệm Tokenizer: phương pháp chuyển đổi dữ liệu text sang dữ liệu số
Có nhiều phương pháp để tạo token, cách đơn giản nhất là tách các từ trong câu thành các token và chuyển đôi chúng sang dạng số.
Ví dụ câu "Jim Henson was a puppeteer" được tách thành các từ ['Jim', 'Henson', 'was', 'a', 'puppeteer'] 

Dự đoán token: trong các mô hình NLP, mỗi câu là một dãy tuần tự các từ (token) do vậy việc dự đoán chính xác token tiếp theo dựa trên dãy các token đã có (input) là rất quan trọng.
Các mô hình LLM đều có khả năng dự đoán token tiếp theo dựa trên dãy các token đầu vào, và token này có thể được sử dụng làm đầu vào cho các dự doán tiếp theo, đây chính là nguyên lý cơ bản
của generative AI cho mô hình xử lý NNTN

4. Nguyên lý làm việc của các mô hình LLM
LLM là một mô hình Generative AI, mô hình này có thể sinh ra các chuỗi văn bản mới dựa trên các dữ liệu đã được huấn luyện và một lới hướng dẫn (instruction) nhằm định hướng kết quả đầu ra mong đợi 
cho LLM hoạt động. Ví dụ:

===============================================








