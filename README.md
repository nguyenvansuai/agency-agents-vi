# Agency Agents — Bản Việt cho doanh nghiệp Việt Nam

Bộ 6 **skill cho Claude** dành cho các mảng mà doanh nghiệp Việt cần nhưng các plugin chuẩn chưa đi sâu: TikTok, livestream bán hàng, sàn TMĐT, quảng cáo mạng xã hội và chăm sóc khách qua Zalo.

Được Việt hóa và **điều chỉnh theo bối cảnh Việt Nam** từ [msitarzewski/agency-agents](https://github.com/msitarzewski/agency-agents). Đây không phải bản dịch máy: các phần về Douyin/WeChat/Amazon đã được chuyển sang TikTok Shop, Shopee, Lazada, Zalo.

Biên soạn bởi **[Sự AI](https://suai.vn)**.

## Danh sách skill

| Skill | Dùng khi | Gốc |
|---|---|---|
| `tiktok-strategist-vn` | Lên kế hoạch kênh TikTok, viết kịch bản video ngắn, chọn KOC | TikTok Strategist |
| `livestream-ban-hang` | Chuẩn bị phiên live, viết kịch bản chốt đơn, đánh giá host, đọc số sau live | Livestream Commerce Coach |
| `van-hanh-san-tmdt` | Tối ưu sản phẩm Shopee/TikTok Shop/Lazada, kế hoạch ngày đôi, tính giá không lỗ | Cross-Border E-Commerce Specialist |
| `quang-cao-mang-xa-hoi` | Chạy Meta Ads/TikTok Ads, phân bổ ngân sách, chẩn đoán ads đắt | Paid Social Strategist |
| `sang-tao-quang-cao` | Viết mẫu quảng cáo, kịch bản video ads, kế hoạch A/B test | Ad Creative Strategist |
| `cham-soc-khach-zalo` | Xây tệp khách trên Zalo OA/nhóm Zalo, kịch bản chăm sóc, kéo mua lại | Private Domain Operator |

## Cài vào app Claude (claude.ai / desktop)

1. Vào thư mục [`dist/`](dist/), tải file `.zip` của skill cần dùng.
2. Trong Claude: bấm **"+"** → **"+ Create skill"** → **"Upload a skill"** → chọn file `.zip`.
3. Xong. Claude tự gọi skill khi yêu cầu khớp mô tả, ví dụ: *"Viết kịch bản livestream bán son cho tối nay"*.

> Chỉ cài skill bạn thật sự cần. Cài quá nhiều skill chồng chéo làm Claude khó chọn đúng.

## Cài vào Claude Code

```bash
git clone https://github.com/nguyenvansuai/agency-agents-vi.git
cp -r agency-agents-vi/skills/* ~/.claude/skills/
```

## Tùy chỉnh cho doanh nghiệp của bạn

Mở `SKILL.md` và thêm vào đầu nội dung các thông tin riêng: ngành hàng, sản phẩm chủ lực, giọng thương hiệu, chính sách đổi trả… Sau đó nén lại **cả thư mục** (tên thư mục phải trùng `name` trong `SKILL.md`) và upload lại.

## Lưu ý

- Đây là **prompt định hướng cách làm việc**, không thêm kiến thức hay công cụ mới cho Claude.
- Chính sách sàn, nền tảng quảng cáo, Zalo và quy định pháp luật thay đổi thường xuyên — luôn đối chiếu nguồn chính thức trước khi áp dụng.
- Các chỉ số trong skill là **mốc tham khảo**, cần hiệu chỉnh theo ngành và số liệu thật của bạn.

## Giấy phép

MIT — xem [LICENSE](LICENSE). Giữ nguyên ghi công tác giả gốc khi sao chép/chỉnh sửa.
