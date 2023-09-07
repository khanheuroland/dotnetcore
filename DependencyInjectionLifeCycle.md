# Quản lý vòng đời (lifetime) Service #
Bất cứ khi nào chúng ta yêu cầu service, DI Container sẽ quyết định xem có tạo mới một thể hiện (instance) hay sử dụng lại thể hiện đã tạo từ trước đó. Vòng đời của Service phụ thuộc vào khi khởi tạo thể hiện và nó tồn tại bao lâu. Chúng ta định nghĩa vòng đời khi đăng ký service.

Chúng ta đã học cách sử dụng DI ở bài trước. Có 3 mức độ vòng đời, bằng cách này chúng ta có thể quyết định mỗi service có vòng đời ra sao.

 - Transient: Một thể hiện mới luôn được tạo, mỗi khi được yêu cầu.
 - Scoped: Tạo một thể hiện mới cho tất cả các scope (Mỗi request là một scope). Trong scope thì service được dùng lại
 - Singleton: Service được tạo chỉ một lần duy nhất.
