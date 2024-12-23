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

3. Khái niệm Tokenizer: phương pháp tách các câu thành các từ riêng lẻ
Có nhiều phương pháp để tạo token, cách đơn giản nhất là tách các từ trong câu thành các token và chuyển đôi chúng sang dạng số.
Ví dụ câu "Jim Henson was a puppeteer" được tách thành các từ ['Jim', 'Henson', 'was', 'a', 'puppeteer'] 

Dự đoán token: trong các mô hình NLP, mỗi câu là một dãy tuần tự các từ (token) do vậy việc dự đoán chính xác token tiếp theo dựa trên dãy các token đã có (input) là rất quan trọng.
Các mô hình LLM đều có khả năng dự đoán token tiếp theo dựa trên dãy các token đầu vào, và token này có thể được sử dụng làm đầu vào cho các dự doán tiếp theo, đây chính là nguyên lý cơ bản
của generative AI cho mô hình xử lý NNTN

4. Nguyên lý làm việc của các mô hình LLM
LLM là một mô hình Generative AI, mô hình này có thể sinh ra các chuỗi văn bản mới dựa trên các dữ liệu đã được huấn luyện và một lới hướng dẫn (instruction) nhằm định hướng kết quả đầu ra mong đợi 
cho LLM hoạt động. Ví dụ:

===============================================
5. Phân loại các mô hình LLM
LLM có thể được phân lọa dựa trên nhiều tiêu chí khác nhau, như kiến trúc network, dữ liệu huấn luyện, và khả năng ứng dụng.
Phân loại theo dữ liệu chúng ta có các mô hình LLM cho text, audio, video, image,...

Xử lý âm thanh và nhận dạng giọng nói, các mô hình dựa trên Whisper có hiệu quả khá tốt, đây là các model được huấn luyện trên tập dữ liệu với nhiều loại âm thanh và có thể nhận dạng
giọng nới với nhiều ngôn ngữ khác nhau

Dữ liệu hình ảnh: model DALL-E là một mô hình có hiệu quả tốt, model này được phát triển bởi Azure OpenAI 
Text generation: trong lĩnh vực này các model được đánh giá tốt nhất hiện tại là GPT-3, GPT-4 hoặc MIstral
Các model nền tảng: đây là các model AI được xây dựng ra dựa trên một số tiêu chí sau:
+ Chúng được huấn luyện theo các phương pháp unsupervised learning hoặc self-supervised 
+ Là mô hình lớn dựa trên mạng nơ ron với hàng tỷ tham số
+ Chúng được sử dụng làm nền tảng cho việc phát triển các model AI mới dựa trên các kỹ thuật như fine-tuning (tinh chỉnh model)

6. Khai niệm Embedding
Embedding là phương pháp để chuyển đổi dữ liệu text thành dữ liệu số. Embedding giúp các LLM dễ dàng tìm ra mối quan hệ giữa các từ hoặc các câu. Ví dụ mỗi câu có thể
chuyển đổi thành một vector số, mối quan hệ giữa các câu có thể được tính theo khoảng cách cosin giữa hai vector số.
Ví dụ: "Microsoft" -> [8, 2, 5, 0]
7. Một số model LLM

8. Cải thiện chất lượng cho các model LLM
Có 3 phương pháp chính để cải thiện chất lượng của các model LLM khi triển khai trong thực tiễn
Prompt engineering with context: đây là phương pháp đơn giản nhất, phương pháp này chúng ta chỉ cần tạo các chỉ dẫn để cung cấp thêm thông tin cho các mô hình LLM trong quá trình sinh nội dung mới
Retrieval Augmented Generation, RAG: phương pháp này thường sẽ tạo và lưu trữ dữ liệu cho ứng dụng cụ thể trong các hệ quản trị CSDL và sử dụng các phương pháp similarity search để
tìm kiếm các nội dung phù hợp và cung cấp cho mô hình LLM trong quá trình sinh nội dung mới.
Fine-tuned model: đây là phương pháp đòi hỏi kỹ thuật tinh chỉnh model dựa trên tập dữ liệu riêng nhằm tạo ra model mới hiệu quả hơn.

9. Using Generative AI Responsibly















