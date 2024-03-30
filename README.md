<div align="center">
    <img src="./terraformio-ar21.svg" alt="terraform_logo" style="display: block; margin: 0 auto;">
</div> 

## &#x1F530; Install Terraform (with Binary download) on macOS M1

&nbsp;

&#x1F516; Informasi pada perangkat pengguna.<br />

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

&nbsp;

with Binary download
    `[macOS][ARM64]` `https://developer.hashicorp.com/terraform/install`

&nbsp;

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

Pastikan `/usr/local/bin` tersedia juga pada PATH<br />
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

&nbsp;

---

&nbsp;

&nbsp;