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
Sử dụng Generative AI một cách đúng đắn
chúng ta có thể sử dụng Generative AI để sinh ra các câu trả lời hữu ích cho người dùng, tuy nhiên trong một số trường hợp Generative AI cũng sinh ra các kết quả không mong đợi
có thể gay hại cho người sử dụng
 
Vấn đề ảo giác (Hallucinations): là hiện tượng các LLM tạo ra một nội dung hoàn toàn vô nghĩa hoặc sai sự thật dựa trên các nguồn thông tin đã được cung cấp.
Ví dụ chúng ta có câu hỏi: "Who was the sole survivor of Titanic?"
Đây là câu trả lời tưởng chừng rất hoàn hảo, tuy nhiên nó không đúng sự thật, bởi trong vụ tai nạn Titanic có rất nhiều người sống sót, điều này dẫn đến hậu quả là AI không đáng tin cậy

+ Các nội dung có hại: một số hệ thống LLM có thể sinh ra các nội dung có hại cho người sử dụng
Các nội dung có hại:
- Cung cấp hoặc khuyến khích tự làm hại bản thân hoặc gây hại cho một số nhóm khác
- Nội dung mang tính thù hận, hạ thấp nhân phẩm
- Có hành vi bạo lực
- Hiển thị nội dung khiêu dâm
+ Thiếu công bằng
=> Làm thế nào để sử dụng Generative AI một cách đúng đắn
 1) Measure Potential Harms: đo lường tác hại tiềm ẩn: đảm bảo kiểm thử nhiều kịch bản với các context khác nhau được cung cấp cho LLM
 2) Giảm thiểu tác hại tiềm ẩn: có thể triển khai vấn đề này ở 4 lớp khác nhau
 + Model: chọn các model LLM một cách đúng đắn, chú ý rằng các model lớn như GPT 4 có thể gây ra nhiều rủi ro về việc sinh ra các nội dung có hại khi áp dụng chúng vào các trường hợp dữ liệu nhỏ cụ thể
 chính vì vậy chúng ta cần phải tinh chỉnh model khi muốn sử dụng trong các trường hợp cụ thể
 
 + Safety System: xậy dựng hệ thống an toàn với nhiều giải pháp đảm bảo an toàn thông tin cho người sử dụng
 + Metaprompt: là phương pháp giới hạn hoặc định hướng mô hình dựa trên một số hành vi và thông tin.
 + User Experience: trải nghiệm người dùng, nên tạo ra một giao diện tương tác thuận tiện và thân thiện với người sử dụng
 
 BÀI 4: Prompt Engineering Fundamentals
What is Prompt Engineering?: định hướng trả lời cho LLM, là quá trình thiết kế tối ưu hóa đầu vào cho các model LLM nhằm tạo ra câu trả lời chính xác nhất. Có hai giai đoạn
+ Thiết kế lời nhắc (prompt) cho LLM cho các mục đích cụ thể
+ Tinh chỉnh lời nhắc nhằm cải thiện chất lượng câu trả lời
Why do we need Prompt Engineering?: tại sao cần có lời nhắc cho các mô hình LLM
thực tế LLM là các mô hình ngôn ngữ lới, chúng được huấn luyện trên các tập dữ liệu vô cùng lớn, do vậy việc sinh ra các câu trả lời một cách chính xác và nhất quán là không thể. Nguyên nhận chính là do:
+ Phản hồi từ các mô hình LLM là ngẫu nhiên: các mô hình LLM có thể sẽ trả về các câu trả lời khác nhau với cùng một câu hỏi

+ Các mô hình có thể bịa ra các câu trả lời: LLM được huấn luyện trên các tập dữ liệu rất lớn, tuy nhiên chúng vẫn là hữu hạn và có thể thiếu tri thức về câu hỏi do người sử dụng đưa vào, 
khi đó LLM có thể sẽ tự bịa ra các câu trả lời
+ Có nhiều model LLM và khả năng của chúng là khác nhau
  
Fabrications Example (bịa đặt câu trả lời):

*) prompt construction
- Các kỹ thuật xây dựng lới nhắc (Prompt)
- Basic prompt: một dòng text được gửi tới đầu vào cho các mô hình LLM, không cung cấp thêm bất kỳ ngữ cảnh nào khác

- Complex Prompt: đây là các lời nhắc được xây dựng theo cấu trúc Input/Output tương ứng với đầu vào của người sử dụng và phản hồi của LLM
+ Thông báo của hệ thống thiết lập ngữ cảnh cho hành vi của trợ lý ảo
-Instruction Prompt: xây dựng các lời nhắc nhằm mô tả chi tiết về nhiệm vụ cần hoàn thành cho các mô hình LLM

*) Primary Content: nội dung chính
Với mẫu Prompt này, các lời nhắc được chia thành 2 phần: + một lời hướng dẫn, + nội dung có liên quan


 
 






















