![Fortress of the Fallen](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/FotF.png)

## Overview
**Fortress of the Fallen** là một game chiến thuật kết hợp phòng thủ tháp và nhập vai (Tower Defense – RPG – Resource Management). Người chơi vào vai **Tam hoàng tử cuối cùng còn sống sót**, phải tử thủ trong pháo đài cuối cùng chống lại thế lực Hỗn Mang. Mỗi chế độ là một chương truyện riêng biệt, với gameplay thủ thành thời gian thực.

---

## Core Game Loop
![Fortress of the Fallen](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/GameLoop.png)

## Game Modes

| Chế độ        | Đặc điểm |
|---------------|----------|
| **Chế độ 1**  | Dễ. Wave cố định. Luyện tập và làm quen. |
| **Chế độ 2**  | Khó hơn. Wave ngẫu nhiên, nhiều stage hơn. |
| **Chế độ 3**  | Cực khó. Wave ngẫu nhiên, quái có chỉ số cao hơn và có nhiều biến số hơn. |

---

## Game Play
- **Thủ thành thời gian thực**: Bố trí đơn vị thủ thành theo vị trí chiến thuật, xây dựng hàng thủ và kiểm soát tài nguyên.
- **Điều khiển bán tự động**: Người chơi chỉ điều khiển nhân vật chính, các đơn vị còn lại do AI điều khiển theo sơ đồ chiến thuật.
- **Đơn vị chết mất vĩnh viễn**, trừ nhân vật chính. Nếu nhân vật chính chết: thua trận.
- **Chi tiết:**
    - Người chơi chọn sơ đồ chiến thuật trước trận.
    - Các đơn vị có thể **hành động theo vai trò (đỡ đòn, dồn sát thương, hồi máu, phá kỹ năng...)**.
    - Hệ thống **Affinity**, **Karma** ảnh hưởng đến kỹ năng học được và nhánh class mở khóa.

## 👤 Character System
![Character System](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/stats-system.png)

- Level tối đa: **100**
- Hệ thống **chỉ số cơ bản và đặc biệt quyết định class**, không tăng cấp theo level.
- Trang bị có thể **tăng chỉ số để mở class mới** hoặc **kích hoạt kỹ năng độc quyền**.
- Các nhân vật **triệu hồi** cũng có class, skill riêng và tiến hóa riêng.

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

## Class System:
[`class-system.md`](./class-system.md): Chi tiết về hệ thống class, chỉ số unlock, trait ảnh hưởng, kết hợp với chủng tộc.
