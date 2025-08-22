# Milestone Phase 1 – Fortress of the Fallen (3 tháng)

## Mục tiêu
Hoàn thành **prototype chạy được**, với các tính năng:
- Client ↔ Server kết nối.
- Đăng nhập / đăng ký tài khoản.
- Vào đảo cá nhân → spawn nhân vật chính.
- Di chuyển nhân vật.
- Gacha NPC cơ bản (NPC có stats, lưu DB).
- NPC AI đơn giản (làm việc → sinh tài nguyên).

---

## Tháng 1: Nền tảng & Kiến trúc
- Thiết kế kiến trúc Client–Server + MultiServer (UML/diagram).
- Thiết kế database: User, Player, NPC, Island.
- Dựng server.
- Cài đặt Socket API.
- Triển khai Auth Service cơ bản (đăng ký, đăng nhập).
- Tạo Unity project:
  - Scene login.
  - Kết nối server qua Socket.

**Milestone 1**  
- Unity client kết nối server (login OK).  
- User đăng ký/đăng nhập lưu vào MongoDB.  

---

## Tháng 2: Prototype Gameplay cơ bản
- Unity: Scene “Island” (map trống, spawn nhân vật chính).
- Điều khiển di chuyển nhân vật (keyboard input).
- Server: Player Service sync vị trí nhân vật.
- Thiết kế NPC model (STR, DEX, CON, INT, WIS, CHA).
- Server: Gacha NPC → random NPC, lưu DB.
- Client: UI gacha, hiển thị NPC nhận được.

**Milestone 2**  
- Đăng nhập → spawn nhân vật chính trong Island.  
- Nhân vật có thể di chuyển.  
- Gacha NPC hoạt động, NPC lưu vào DB.  

---

## Tháng 3: Tích hợp & Demo Prototype
- Server: NPC AI cơ bản (Farmer → tạo food mỗi 5 phút).
- Client: UI NPC list + HUD cơ bản (HP/MP/Gold).
- Server sync tài nguyên đảo (Gold, Food).
- Kiểm thử client–server với 2–3 client.
- Log sự kiện (login, gacha, NPC hoạt động).

**Milestone 3 (kết thúc Phase 1)**  
- Người chơi có thể:
  1. Đăng nhập.
  2. Vào đảo cá nhân, di chuyển nhân vật.
  3. Gacha NPC (NPC có stats, lưu DB).
  4. NPC làm việc đơn giản (tạo tài nguyên).  
- Báo cáo Phase 1 hoàn chỉnh (thiết kế + demo).  

---

## Tổng kết Phase 1
- **Tháng 1 (Milestone 1):** Client–Server login thành công.  
- **Tháng 2 (Milestone 2):** Di chuyển nhân vật + Gacha NPC.  
- **Tháng 3 (Milestone 3):** NPC AI cơ bản + HUD + demo prototype.  
