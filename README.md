![Fortress of the Fallen](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/FotF.png)

## Overview
**Fortress of the Fallen** là một game chiến thuật kết hợp phòng thủ tháp và nhập vai (Tower Defense – RPG – Resource Management). Trò chơi xoay quanh ba tuyến truyện chính của ba Tam Hoàng Tử, mỗi người đại diện cho một phong cách chơi và triết lý cai trị khác nhau.

---

## Core Game Loop
![Fortress of the Fallen](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/FotF.png)

## Game Modes

### 1. **The Conqueror's Path** - *Chiến tranh và xâm lược*
- **Lối chơi**: Mở rộng lãnh thổ, càn quét quân địch, phát triển quân đội.
- **Tài nguyên chính**: Lính đánh thuê, vàng, lãnh thổ.
- **Mục tiêu**: Chinh phục các vùng đất bị lãng quên và đánh bại các pháo đài địch.

### 2. **The Tyrant’s Fortress** - *Phòng thủ*
- **Lối chơi**: Phòng thủ tháp, tối ưu hóa công trình, quản lý NPC/đơn vị.
- **Tài nguyên chính**: Tinh thể ma thuật, nguyên vật liệu xây dựng, thời gian.
- **Mục tiêu**: Xây dựng pháo đài bất khả xâm phạm chống lại các đợt tấn công.

### 3. **The Schemer’s Dominion** - *Quản trị, mưu lược, ám sát*
- **Lối chơi**: Chính trị, thuyết phục, cạm bẫy, kiểm soát thông tin.
- **Tài nguyên chính**: Thông tin, uy tín, niềm tin, ám sát.
- **Mục tiêu**: Điều khiển thế giới từ trong bóng tối thông qua mạng lưới gián điệp.

---

## 👤 Character System
![Character System](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/stats-system.png)

### A. Base Attributes (Chỉ số cơ bản)

| Attribute | Mô tả |
|----------|-------|
| STR (Strength)     | Sức mạnh cơ bắp, sát thương vật lý |
| DEX (Dexterity)    | Nhanh nhẹn, chính xác, tốc độ đánh |
| CON (Constitution) | Thể lực, máu, kháng sát thương |
| INT (Intelligence) | Trí tuệ, phép thuật, kháng phép |
| WIS (Wisdom)       | Niềm tin, khả năng sử dụng kỹ năng đặc biệt |
| CHA (Charisma)     | Mở khóa các kỹ năng đặc biệt |

### B. Derived Stats (Chỉ số phụ thuộc)

| **Stat**        | **Phụ thuộc vào**         | **Ý nghĩa**                            |
|----------------|---------------------------|----------------------------------------|
| HP             | CON, STR                  | Máu tối đa                              |
| MP             | WIS, INT                  | Mana tối đa                             |
| PATK / DATK    | STR, DEX, CON             | Tấn công / phòng thủ vật lý              |
| MATK / MDEF    | INT, WIS                  | Tấn công phép / kháng phép             |
| SPD            | DEX                       | Tốc độ hành động / đánh                |
| CRIT           | DEX                       | Tỷ lệ chí mạng                          |
| ACC            | DEX, INT                  | Độ chính xác khi tấn công              |
| EVA            | DEX, CON                  | Né tránh đòn đánh                      |

### C. Special Traits (Thuộc tính đặc biệt)

| Trait       | Mô tả |
|-------------|-------|
| Karma       | Đạo đức nhân vật (tốt, ác, trung lập) ảnh hưởng đến kỹ năng, mối quan hệ |
| Affinity    | Mối liên kết với phe phái / nguyên tố / NPC |
| Luck        | Tác động đến tỷ lệ rơi đồ, chí mạng, sự kiện ngẫu nhiên |
| Resistance  | Khả năng chống lại hiệu ứng bất lợi (poison, stun, curse...) |

---

## Race & Stat Cap System (Chủng tộc và giới hạn chỉ số)

Mỗi **chủng tộc** sẽ có:
- **Giới hạn chỉ số khác nhau**
- **Kháng / yếu với các nguyên tố**
- **Thế mạnh riêng biệt** trong lối chơi

### Ví dụ

| Race        | STR | DEX | CON | INT | WIS | CHA | Ghi chú |
|-------------|-----|-----|-----|-----|-----|-----|--------|
| Human       | 8   | 8   | 8   | 8   | 8   | 8   | Cân bằng |
| Elf         | 6   | 10  | 6   | 10  | 10  | 8   | Giỏi phép, tốc độ cao |
| Orc         | 12  | 6   | 10  | 4   | 4   | 4   | Cận chiến mạnh, kháng vật lý |
| Undead      | 6   | 6   | 12  | 8   | 6   | 4   | Không hồi máu, miễn độc |
| Dragonkin   | 10  | 10  | 10  | 10  | 10  | 6   | Rất mạnh nhưng tăng cấp chậm |

> Giới hạn có thể được tăng qua tiến hóa, tăng cấp, hoặc vật phẩm huyền thoại.

---

## Resource Management System

### Tài nguyên chính:
- **Gold**: Dùng để nâng cấp công trình, thuê lính, mua trang bị.
- **Mana Crystals**: Dùng để thi triển phép, nâng cấp công nghệ ma thuật.
- **Soul Shards**: Đơn vị hiếm, dùng để triệu hồi anh hùng, kỹ năng tối thượng.
- **Influence**: Chỉ số ảnh hưởng chính trị / uy tín nhân vật trong faction.

---