# 使用S3的步驟
1.在S3創一個bucket

2.創造一個網站(html)然後上傳到S3

3.在"屬性"中的"儲存貯體版本控制"把版本控制打開

4.之後更改網站內容後再次上傳

5.在"物件"中打開列出版本後就能看到所有的版本

6.到"屬性"中啟用靜態網站託管

7.到"許可"封鎖公有存取權"中把"封鎖所有公開存取權"關掉

8.到下面的"儲存貯體政策"把程式碼複製過去後更改resource成自己

## 第8步驟的程式碼
{
  "Version":"2012-10-17",
  "Statement":[
    {
      "Sid":"PublicRead",
      "Effect":"Allow",
      "Principal": "*",
      "Action":["s3:GetObject","s3:GetObjectVersion"],
      "Resource":["arn:aws:s3:::DOC-EXAMPLE-BUCKET/*"]
    }
  ]
}

# 使用Amplify的步驟
1.Host your web app"選擇Github

2.跟Github做連接

[HW3的連結](https://youtu.be/MmwaIeQlFqM)
