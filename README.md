**Cách built 1 framework cypress trên typescript**
1. Gõ câu lệnh **npm init -y** , sau khi gõ xong sẽ sinh ra 1 file **package.json**
2. Gõ câu lệnh **npm install cypress --save-dev** để cài đặt thư viện cypress
3. Gõ câu lệnh **npx cypress open** để mở cypress lên, sau khi mở xong sẽ sinh ra thư mục **cypress**, trong thư mục cypress chứa 2 thư mục con là **fixture** và **report**, và thêm 1 file **cypress.config.js**
4. Vào file **cypress.config.js** chỉnh sửa đường dẫn để chạy test bằng cách thêm câu lệnh sau **specPattern:"./cypress/Testcase/Home/**.*"** đường dẫn này sẽ tùy theo cấu hình của mình
5. **=> Đến đây coi như là cấu hình xong 1 dự án cypress**
6. Copy file **tsconfig.json**
7. Vào file **tsconfig.json** chỉnh sửa đường dẫn nơi mà mình biên dịch file ts ở câu lệnh **"include": ["cypress/**/*.ts"]**, tùy theo cấu hình dự án mà mình thay đổi cho thích hợp
8. Cài nốt 2 thư viện của typescript và cypress buitl trên typescript: **npm install @types/cypress --save-dev** và **npm install typescript --save-dev**
9. Viết 1 test mẫu
10. Chạy test bằng câu lệnh **npx cypress open**