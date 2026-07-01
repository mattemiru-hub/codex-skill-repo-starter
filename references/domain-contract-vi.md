# Domain Contract - Repo Skill Starter

File này định nghĩa rõ repo này phải tạo ra cái gì khi user muốn dựng hoặc polish một repo skill Codex.

## Mục tiêu

- tạo ra repo skill Codex có cấu trúc rõ ràng, có thể share lên GitHub và cài local để dùng ngay
- tách bạch repo bootstrap khỏi repo domain nếu hai boundary này đang bị trộn
- đảm bảo repo mới có đủ `SKILL.md`, `references/`, script cài đặt, tài liệu hướng dẫn và checklist QA

## Đầu ra cuối cùng phải có

- `SKILL.md` đúng scope và trigger
- `README.md` và nếu cần thì `README_vi.md`
- `agents/openai.yaml`
- `references/` đủ cho clarification, contract, prompt, QA
- `scripts/install_local_skill.ps1`
- nếu repo là starter repo thì có thêm script scaffold như `init_standard_skill_repo.ps1`
- ví dụ và sample-output nếu chúng thực sự giúp người dùng tái sử dụng

## Workflow bắt buộc

1. xác định repo này là repo domain hay repo bootstrap
2. kiểm tra user muốn dùng repo để build mới, polish, audit hay đóng gói
3. chốt những file và thư mục bắt buộc của repo
4. viết hoặc chỉnh `SKILL.md` để AI biết lúc nào phải dùng skill và hỏi lại khi mơ hồ
5. bổ sung README, references, scripts và metadata để repo dùng được trên GitHub và local Codex
6. audit lại wording, placeholder, logic trigger và install flow trước khi bàn giao

## Non-negotiables

- không trộn logic bootstrap vào repo domain nếu nó nên sống ở repo riêng
- không để placeholder lộ liễu trong README, references hoặc changelog nếu repo đã public
- không viết `SKILL.md` mơ hồ đến mức AI phải đoán scope hoặc output
- nếu install flow, boundary hoặc deliverable còn mơ hồ thì phải hỏi lại
