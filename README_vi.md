# Codex Skill Repo Starter - Bản Tiếng Việt

Đây là repo starter riêng để tạo ra các repo skill Codex hoàn chỉnh, không phải repo domain nghiệp vụ cuối cùng.

## Repo này có gì

- `SKILL.md` để Codex biết khi nào phải dùng skill
- luật hỏi lại trước khi đoán
- tài liệu tham chiếu trong `references/`
- ví dụ dùng trong `examples/`
- ghi chú đầu ra mẫu trong `sample-output/`
- script cài nhanh vào thư mục skill local
- script sinh repo chuẩn mới

## Cách dùng nhanh

1. Cài skill bằng `scripts/install_local_skill.ps1`
2. Gọi Codex với cú pháp `$codex-skill-repo-starter`
3. Mô tả repo skill mới bạn muốn tạo
4. Để skill tự hỏi lại các thông tin còn mơ hồ rồi dựng repo
5. Hoặc chạy `scripts/init_standard_skill_repo.ps1` để có ngay một scaffold local

## Repo này nên dùng khi nào

- khi bạn muốn tạo repo skill mới từ đầu
- khi bạn muốn ép AI dựng repo theo đúng bộ khung chuẩn
- khi bạn muốn tách riêng phần bootstrap repo khỏi repo domain chính

## Cần chỉnh gì sau khi sinh repo mới

- thay mô tả skill theo domain thật
- điền lại `references/domain-contract-vi.md`
- điền lại `references/prompt-template-vi.md`
- bổ sung checklist QA thật sự dùng được
- thay ví dụ và sample output bằng output thật của repo
