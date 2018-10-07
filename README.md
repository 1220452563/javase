package com.work03.Test;

import java.net.InetAddress;
import java.net.UnknownHostException;

public class InetAddressTest {

	public static void main(String[] args) throws UnknownHostException {
		// IP地址对象InetAddress
		// 获取本地主机对象
		InetAddress IP = InetAddress.getLocalHost();
		System.out.println(IP.getHostAddress()+" :←IP地址--计算机名称→: "+IP.getHostName());
		// 获取其他主机的地址对象(通过指定的IP或者主机名获取)
		InetAddress ip = InetAddress.getByName("www.baidu.com.cn");
		System.out.println(ip.getHostAddress()+" :←IP地址--计算机名称→: "+ip.getHostName());

	}

}
