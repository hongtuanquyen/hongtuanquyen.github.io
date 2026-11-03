# hongtuanquyen.github.io

# Links
Base URL: https://hongtuanquyen.github.io/

| File | Link |
|---|---|
| index.html (mục lục) | https://hongtuanquyen.github.io/ |
| sa/security-roadmap.html | https://hongtuanquyen.github.io/sa/security-roadmap.html |
| sa/certification-guide.html | https://hongtuanquyen.github.io/sa/certification-guide.html |
| sa/interview-mastery.html | https://hongtuanquyen.github.io/sa/interview-mastery.html |
| .well-known/assetlinks.json | https://hongtuanquyen.github.io/.well-known/assetlinks.json |
| .well-known/apple-app-site-association | https://hongtuanquyen.github.io/.well-known/apple-app-site-association |

- `sa/` = Software Architecture.
- Có thể bỏ đuôi `.html`, ví dụ: https://hongtuanquyen.github.io/sa/security-roadmap
- Khi thêm route mới, nhớ thêm link vào `index.html` (mục lục) và bảng trên.
- Sau khi push lên `main`, GitHub Pages build lại mất khoảng 1 phút.

# .well-known folder
Nếu sử dụng Firebase Dynamic Links (FALs), assetlinks.json và apple-app-site-association là không cần thiết.
Ngược lại, nếu config Applinks (Android) và Universal link (iOS) mà ko dùng FALs thì cần assetlinks.json và apple-app-site-association.

Jekyll mặc định bỏ qua thư mục bắt đầu bằng dấu `.`, nên cần `include: [".well-known"]` trong `_config.yml` để folder này được publish.
