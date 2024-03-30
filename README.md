<div align="center">
    <img src="./terraformio-ar21.svg" alt="terraform_logo" style="display: block; margin: 0 auto;">
</div> 

## &#x1F530; Install Terraform (with Binary download) on macOS M1

&nbsp;

&#x1F516; Information on the user's device.<br />

<pre>
    ❯ system_profiler SPSoftwareDataType SPHardwareDataType

        Software:
            System Software Overview:
                System Version: macOS 13.3.1 (22E261)
                Kernel Version: Darwin 22.4.0
                Boot Volume: Macintosh HD
                Boot Mode: Normal    
                . . .

        Hardware:
            Hardware Overview:
                Model Name: MacBook Pro
                Model Identifier: MacBookPro17,1
                Model Number: MYD82ID/A
                Chip: Apple M1
                Total Number of Cores: 8 (4 performance and 4 efficiency)
                Memory: 8 GB
                . . .
</pre>

&nbsp;


## &#x1F530; Begin.

<pre>
    ❯ pwd
        /Users/&lt;user&gt;

</pre>

---

with Binary download :<br />
&emsp; &emsp; &emsp; `[macOS][ARM64]` `https://developer.hashicorp.com/terraform/install`

---

<pre>
    ❯ ls -lah | grep terraform

        -rwxr-xr-x@   1 &lt;user&gt;  staff    89M Mar 18 15:53 terraform
</pre>
<pre>
    ❯ sudo mv terraform /usr/local/bin

    ❯ ls -lah /usr/local/bin  | grep terraform

            -rwxr-xr-x@  1 &lt;user&gt;  staff    89M Mar 18 15:53 terraform
</pre>

&nbsp;

Make sure `/usr/local/bin` is also available in the PATH<br />
- output :<br /><br />
    /Users/.../bin:...:/usr/local/bin:/System/Cryptexes/App/usr/bin:/usr/...

<pre>
    ❯ terraform --version

        Terraform v1.7.5
        on darwin_arm64
</pre>

&#x1F31F; &#x1F31F;[DONE] &#x1F31F; &#x1F31F;

&nbsp;

---

&nbsp;

&nbsp;

<div align="center">
    <img src="./ss_terraform_logo.png" alt="ss_terraform_logo" style="display: block; margin: 0 auto;">
</div> 

&nbsp;

---

**Documentation [Bahasa Indonesia]**

Reference :<br />
<pre>https://sanimuhlison.medium.com/terraform-untuk-pemula-dccf947817c5</pre>

## Terraform Untuk Pemula

&nbsp;

### Apa itu Terraform ?

**Terraform** adalah tool open source untuk membangun, mengubah dan membuat versi infrastructure dengan aman dan efisien. Biasanya dikenal dengan infrastructure as code. Terraform dibuat oleh HashiCorp.

&nbsp;

**Core Terraform Workflow** <br />

Ada 3 tahapan inti didalam alur kerja terraform, yaitu :

**WRITE → PLAN → APPLY**

- **Write:** Tulis terraform configuration dan initialize

    Anda bisa menulis code didalam terraform configuration file ( .tf ), kemudian lakukan initialize dengan command `terraform init` .

- **Plan:** Preview

    Sebelum diterapkan ke infrastructure yang sebenarnya, anda bisa melakukan preview terlebih dahulu apa yang akan dibuat, ubah atau hapus sehingga lebih aman saat diterapkan ke infrastructure yang sebenarnya.

- **Apply:** Terapkan ke real infrastructure

    Setelah anda review, anda bisa menerapkan ke infrastructure yang sebenarnya dengan command `terraform apply` .

&nbsp;

&nbsp;

**Terraform Command** <br />

Ada banyak <i>terraform command</i> yang bisa anda gunakan, tetapi disini saya akan menjelaskan beberapa command dasar yang umum digunakan untuk pemula. Untuk command lainnya bisa anda lihat <a href="https://developer.hashicorp.com/terraform/cli/commands">disini</a>. Beberapa command dasar yang umum digunakan untuk pemula adalah sebagai berikut: