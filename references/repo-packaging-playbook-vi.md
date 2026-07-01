# Playbook Đóng Gói Repo Skill Hoàn Chỉnh

File này là checklist để dựng một repo skill hoàn chỉnh ngay từ đầu, tránh kiểu làm xong mới vá dần.

## 1. Chốt boundary của repo

Ngay từ đầu phải chốt:

- đây là repo domain hay repo bootstrap
- repo này dùng để build mới, polish, audit, hay đóng gói
- phần nào phải ở repo riêng, không được trộn

## 2. Bộ khung tối thiểu

Một repo skill dùng thật nên có:

- `SKILL.md`
- `README.md`
- `README_vi.md` nếu user chính là tiếng Việt
- `references/`
- `scripts/`
- `examples/`
- `sample-output/`
- `CHANGELOG.md`
- `LICENSE`
- `agents/openai.yaml`

## 3. Các lớp bắt buộc

Repo tốt phải đủ 4 lớp:

- hướng dẫn dùng
- luật vận hành
- tài liệu tham chiếu
- kiểm thử cài và hành vi

## 4. Clarification-first

Skill phải biết hỏi lại khi:

- không rõ boundary của repo
- không rõ install flow
- không rõ output cuối cùng
- không rõ phần nào là domain-specific, phần nào là bootstrap

## 5. Test bắt buộc

Trước khi coi repo là ổn, phải test:

- cài từ GitHub
- cài local bằng script nếu có
- mở được `SKILL.md`
- skill có trigger đúng
- AI có hỏi lại khi gặp chỗ mơ hồ
