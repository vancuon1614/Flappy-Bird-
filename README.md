# GIỚI THIỆU
- Đây là một game 2D thuộc thể loại Endless Runner lấy cảm hứng từ Flappy Bird Người chơi điều khiển Bird bay qua các chướng ngại vật liên tục xuất hiện, với mục tiêu đạt điểm số cao nhất có thể
- Game được xây dựng bằng Unity và sử dụng Visual Scripting (Flow Graph / Activity) để xử lý logic 
# GAMEPLAY
- Người chơi nhấn phím (hoặc click chuột) để điều khiển Bird bay lên
- Trọng lực sẽ kéo Bird xuống liên tục
- Nhiệm vụ là né các ống (pipes) xuất hiện ngẫu nhiên
- Mỗi lần vượt qua một chướng ngại vật, người chơi sẽ được cộng điểm
- Game kết thúc khi va chạm với chướng ngại vật hoặc rơi xuống đất

# CÔNG NGHỆ SỬ DỤNG
- Unity Engine
- Visual Scripting (Unity Visual Scripting - Flow Graph)
- 2D Physics System (Collider, Rigidbody)

# CÁCH HOẠT ĐỘNG
Game được xây dựng hoàn toàn bằng Flow Activity trong Visual Scripting:
- Input System: Bắt sự kiện click/nhấn phím để tạo lực đẩy lên cho Bird
- Physics Handling: Sử dụng Rigidbody2D để áp dụng trọng lực và lực bay
- Obstacle Spawning: Các chướng ngại vật được sinh ra theo thời gian bằng loop (Timer / Coroutine equivalent trong Flow)
- Collision Detection: Sử dụng OnCollision / OnTrigger để phát hiện va chạm. Nếu va chạm thì kích hoạt Event Game Over
- Score System: Tăng điểm khi Bird vượt qua pipe (Trigger zone)
- Game State: Quản lý trạng thái: Start / Playing / Game Over bằng biến trong Flow Graph để diều khiển luồng game

# CẤU TRÚC CHÍNH
<pre>
Assets/ | — Scenes/ | — Scripts (Visual Scripting Graphs) | — Prefabs/ | — Sprites/ | — Audio/
</pre>

# CÁCH CHẠY PROJECT
- Mở project bằng Unity Hub
- Load scene chính (Main Scene)
- Nhấn Play để bắt đầu game

# TÍNH NĂNG NỔI BẬT
- Gameplay đơn giản, dễ tiếp cận
- Thiết kế tối ưu cho học tập và demo cơ chế game loop
- 
# HƯỚNG PHÁT TRIỂN
- Thêm menu (Start / Restart / Pause)
- Lưu điểm cao (High Score)
- Hiệu ứng âm thanh và animation
- Tăng độ khó theo thời gian

## Project phục vụ mục đích học tập và nghiên cứu về Visual Scripting trong Unity
