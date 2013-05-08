BaiduPush Server SDK
====================

百度云推送服务端接口的 java 实现

使用方法:

	import cn.oopsware.baidupush.*;
	
	public class test {
	
		private final static String USERID = "xxxxxxxxxxxxx";
		private final static String CHANNELID = "xxxxxxxxxxxxxxxxxxx";
		
		private final static String API_KEY = "xxxxxxxxxxxxxxxxxxxxxxxx";
		private final static String SECRIT_KEY = "xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";
		
		public static void main(String[] args) {
			BaiduPush baiduPush = new BaiduPush(BaiduPush.HTTP_METHOD_POST, SECRIT_KEY, API_KEY);
			
			//System.out.format("PUSH: %s\n", baiduPush.QueryBindlist(USERID, CHANNELID));
			//System.out.format("PUSH: %s\n", baiduPush.VerifyBind(USERID, null));
			
			//System.out.format("PUSH: %s\n", baiduPush.SetTag("tag1"));
			//System.out.format("PUSH: %s\n", baiduPush.SetTag("tag2"));
			//System.out.format("PUSH: %s\n", baiduPush.SetTag("tag3"));
			
			//System.out.format("PUSH: %s\n", baiduPush.QueryUserTag(USERID));
			//System.out.format("PUSH: %s\n", baiduPush.FetchTag());
			
			System.out.format("PUSH: %s\n", baiduPush.PushMessage("hello world"));
			//System.out.format("PUSH: %s\n", baiduPush.PushMessage("hello world", USERID));
			//System.out.format("PUSH: %s\n", baiduPush.PushTagMessage("hello", "tag1"));
			
			//System.out.format("PUSH: %s\n", baiduPush.PushNotify("Hello", "hello world", USERID));
					
		}
	
	}

