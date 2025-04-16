# RVCK ( RISC-V Common Kernel ) 

RISC-V 内核同源项目 

## 简介

RVCK 内核同源项目（也称 RVCK）是 kernel.org 以及 openEuler 等 linux 内核分支的下游，旨在为目前基于不同硬件平台的 RISC-V 开发生态提供一个统一的内核平台，维护公共开发演进需求，减少维护复杂度并增强软硬件上下游生态协同能力。

由于现有厂商内核版本与 kernel 6.6 较为接近，并且实现统一适配的技术难度较低。RVCK 目前的主要开发基座基于 Kernel6.6 版本，从 ServerPlatform 到内核 6.6 中间存在大量的移植工作，以及相应的测试与优化工作由 RVCK 项目负责。

RVCK 项目目前已经与 openEuler Kernel SIG 建立合作，所有经过验证的开发结果都会同步合入 openEuler OLK 项目。

### 已经合并的平台

| 厂商     | SOC    | 开发板         |
| -------- | ------ | -------------- |
| 算能     | SG2042 | Milk-V Pioneer |
| 平头哥   | TH1520 | LicheePi 4A    |
| 进迭时空 | K1     | Key Stone K1   |

## 贡献过程

![贡献过程](../image/patch-flow.png)

虚线框内为 rvck-olk 项目的范畴，左边是厂商的代码，右边对接 openEuler 主线内核仓库。大致贡献过程是：

* 厂商首先整理代码，主要是通过 checkpatch.pl 测试和剔除商业代码；
* 新建一个 issue;
* 发起 pull requests 并关联 issue；
* 补丁通过 RAVA 项目自动化测试；
* 人工审核代码是否符合 rvck 规范并确保代码质量；
* 最后合并进 rvck-olk 仓库的 OLK-6.6 分支；
* 稳定后我们会 release 至 src 发版仓库，该仓库为 openEuler OS 打包仓库；
* openEuler Kernel SIG 成员将及时合并的的补丁集提交到 openEuler 主线内核 OLK-6.6 分支。
  
## 如何开始
  
  [贡献手册](https://github.com/RVCK-Project/rvck-olk/wiki)
  
  扫描微信二维码联系中科院软件所 王经纬:
<!-- 微信二维码部分 -->
<div align="center" style="margin-bottom: 40px;">
  <img src="../image/wechat-jingwiw.png" alt="王经纬微信" width="400" height="500" style="max-width: 100%; height: auto;">
</div>

<!-- 合作单位标题 -->
## 合作单位

<!-- 合作单位列表 -->


<!-- 第一层：SpacemiT, Sophgo, Sipeed -->
<table align="center" style="margin-bottom: 20px;">
  <tr>
    <td align="center" style="padding: 0 10px;">
      <img src="../image/partner/spacemit.png" alt="SpacemiT" style="max-width: 150px; width: 100%; height: auto;">
    </td>
    <td align="center" style="padding: 0 10px;">
      <img src="../image/partner/sophgo.png" alt="Sophgo" style="max-width: 150px; width: 100%; height: auto;">
    </td>
    <td align="center" style="padding: 0 10px;">
      <img src="../image/partner/sipeed.png" alt="Sipeed" style="max-width: 150px; width: 100%; height: auto;">
    </td>
  </tr>
</table>

<!-- 第二层：openEuler, OERV -->
<!-- 第二层：openEuler, OERV -->
<table align="center" style="margin-bottom: 20px;">
  <tr>
    <td align="center" style="padding: 0 10px;">
      <!-- 固定尺寸容器 -->
      <div style="width: 150px; height: 150px; display: flex; align-items: center; justify-content: center;">
        <img src="../image/partner/openeuler.png" alt="openEuler" style="max-width: 100%; max-height: 100%; object-fit: contain;">
      </div>
    </td>
    <td align="center" style="padding: 0 10px;">
      <!-- 固定尺寸容器 -->
      <div style="width: 150px; height: 150px; display: flex; align-items: center; justify-content: center;">
        <img src="../image/partner/oerv.png" alt="OERV" style="max-width: 100%; max-height: 100%; object-fit: contain;">
      </div>
    </td>
  </tr>
</table>

<!-- 第三层：ISCAS -->
<table align="center">
  <tr>
    <td align="center" style="padding: 0 10px;">
      <img src="../image/partner/iscas.svg" alt="ISCAS" style="max-width: 150px; width: 100%; height: auto;">
    </td>
  </tr>
</table>