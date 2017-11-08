# 计算机网络

## 第一章

### 计算机网络概述

计算机网络的性能指标：

1. 带宽

2. 时延

 1. 发送时延：从发送分组的第一个比特起，至该分组最后一个比特发送完毕所需的时间，也称传输时延。传输时延=分组长度/信道宽度
 1. 传播时延：一个比特从链路一端传到另一端所需的时间。传播时延=信道长度/电磁波在信道上的传播速率
3. 时延带宽积
4. 往返时延
5. 吞吐量
6. 速率 

计算机网络体系结构与参考模型

<p style="text-indent:2em;">
	<table style="width:100%;" cellpadding="2" cellspacing="0" border="1" bordercolor="#000000">
		<tbody>
			<tr>
				<td colspan="8" style="text-align:center;">
					<p align="center">
						<span>OSI模型</span> 
					</p>
				</td>
			</tr>
			<tr>
				<td style="text-align:center;" rowspan="2">
				</td>
				<td style="text-align:center;" colspan="3">
					<p align="center">
						<span>通信子网</span> 
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;" colspan="3">
					<p align="center">
						<span>资源子网</span>
					</p>
				</td>
			</tr>
			<tr>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>物理层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>数据链路层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>网络层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>传输层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>会话层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>表示层</span>
					</p>
				</td>
				<td style="text-align:center;background-color:#E53333;">
					<p align="center">
						<span>应用层</span>
					</p>
				</td>
			</tr>
			<tr>
				<td style="text-align:center;">
					<p align="center">
						<span>传输单位</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span style="color:#E53333;">比特</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span style="color:#E53333;">帧</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span style="color:#E53333;">数据报</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>报文</span><span style="color:#E53333;">段</span><span>（TCP）或用户数据<span style="color:#E53333;">报</span><span>（UDP）</span>
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
			</tr>
			<tr>
				<td style="text-align:center;">
					<p align="center">
						<span><span>任务</span> </span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>透明地传输比特流</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>将网络层传下来的IP数据报组装成帧</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>把网络层的协议数据单元（分组）从源端传到目的端，为分组交换网上的不同主机提供通信服务</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>负责主机中两个进程之间的通信，为</span><span style="color:#E53333;">端到端</span><span>连接提供可靠的传输服务</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>负责管理主机间的会化进程，包括建立、管理以及终止进程间的会话。</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>处理在两个通信系统中交换信息的表示方式</span>
					</p>
<br />
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>为特定类型的网络应用提供访问OSI环境的手段</span>
					</p>
<br />
				</td>
			</tr>
			<tr>
				<td style="text-align:center;">
					<p align="center">
						<span><span>功能</span> </span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>在物理媒体上为数据端设备透明地传输原始比特流</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>成帧、差错控制、流量控制、传输管理</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>流量控制、拥塞控制、差错控制、网际互联</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>为</span><span><span style="color:#E53333;">端到端</span>连接提供流量控制、差错控制、服务质量、数据传输管理</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>同步、校验点</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>数据表示变换：数据压缩、加密解密</span>
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
			</tr>
			<tr>
				<td style="text-align:center;">
					<span>协议</span><br />
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>EIA-232C、EIA/TIA、RS-449 CCITT.X.21</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>SDLC、HDLC、PPP、STP、帧中继</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>IP、IPX、ICMP、IGMP、ARP、RARP、OSPF</span>
					</p>
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>TCP、UDP</span>
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>FTP、SMTP、HTTP</span>
					</p>
				</td>
			</tr>
			<tr>
				<td style="text-align:center;">
					<p align="center">
						<span>其他</span> 
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<p align="center">
						<span>使用校验点继续恢复通信</span>
					</p>
				</td>
				<td style="text-align:center;">
					<br />
				</td>
				<td style="text-align:center;">
					<br />
				</td>
			</tr>
		</tbody>
	</table>
</p>

OSI参考模型在网络层支持无连接和面向连接的通信，但在传输层仅有面向连接的通信；
而TCP/IP模型在网际层仅有一种无连接的通信模式，但在传输层支持无连接和面向连接两种模式。
