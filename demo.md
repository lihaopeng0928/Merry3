graph TD;
    A[开始] --> B[获取当前Token];
    B --> C[显示输入框];
    C --> D[处理用户输入];
    D --> E{用户点击取消?};
    E -- 是 --> F[结束];
    E -- 否 --> G{用户输入新的Token?};
    G -- 否 --> F;
    G -- 是 --> H[更新Token];
    H --> I[结束];