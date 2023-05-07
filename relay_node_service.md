## Thông tin về Relay Node của Biconomy

- **Relay Node** chịu trách nhiệm cho việc xác định các "Transaction" hợp lệ, trả cho người dùng "Gas fees".
- Hỗ trợ gửi "Transactions" và quản lí việc kí transaction, quản lí nonce, ước tính giá gas, gửi lại transaction (**Resubmission**)

## Kiến trúc

- **Common**: Bao gồm tất cả các dịch vụ mà sẽ được chia sẻ bởi "Models" của dự án. Bao gồm cơ sở dữ liệu, bộ nhớ cache, dịch vụ giá gas, dịch vụ mạng, bộ ghi chép v.v.

- **Server**: Bao gồm tất cả các đường dẫn (routes) cùng với các phương pháp xác thực dữ liệu đầu vào và kiểm tra thông qua "Middleware".

- **Relayer**: Chứa các logic cốt lõi của quản lý và xử lý giao dịch của Relayer. Phần này cũng chịu trách nhiệm đối với việc gửi lại giao dịch và thông báo cho "Client" về trạng thái của giao dịch.

## References:

1. https://2292242862-files.gitbook.io/~/files/v0/b/gitbook-x-prod.appspot.com/o/spaces%2FIi3tpVbpF01vBC8NJtcj%2Fuploads%2FVpQZNdTDwoVwW1ytCrqJ%2FRelayer%20Node%20Architecture%20Diagram.drawio.png?alt=media&token=dd626f06-19a7-471e-a218-0e05068a169a
