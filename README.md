# helloworld
package utils;

import android.content.Context;

/**
 * 网络缓存的工具类
 * Created by XMZ on 2016/5/14.
 */
public class CatchUtils {
   /**
    * 以url为key，以json为value，保存到本地
    */

   public static void setCatch(String url, String json, Context ctx) {
      PrefUtils.setString(ctx, url, json);


   }

   public  static String getCatch(String url, Context ctx) {

      return PrefUtils.getString(ctx, url, null);
   }

}
