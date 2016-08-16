 *	云犀直播PHP-SDK, 官方API部分
 *  @author  holger <whjsjq@gmail.com>
 *  @link
 *  @version 1.0

 * 手动引入
 * require_once('/path/to/Yunxizhibo-php/Yunxizhibo.php');

 *  usage:
 *   $accessKey = 'accessKey';  //填写加密用的AccessKey
 *   $secretKey = 'secretKey';  //填写解密用的SecretKey
 *	 $yxObj = new Yunxizhibo($accessKey, $secretKey);
 *
 *   //获取活动列表
 *   $data = $yxObj->getActivityList();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $list = $data["activitys"];  //列表
 *
 *  $pageCount = $data["pageCount"]; //页数
 *
 *   //获取活动资料
 *   $data = $yxObj->getActivityInfo();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $activity = $data["activity"]; //活动详情
 *
 *
 *
 *   //获取直播视频资料
 *   $data = $yxObj->getLivestreamInfo();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $livestream = $data["livestream"];  //直播视频详情
 *
 *  $wechatPlayUrl = $data["wechatPlayUrl"]; //微信嵌入地址
 *
 *  $webPlayUrl = $data["webPlayUrl"]; //网页嵌入地址
 *
 *  $appPlayUrl = $data["appPlayUrl"]; //app嵌入地址
 *
 *  $embedPlayerUrl = $data["embedPlayerUrl"]; //播放器嵌入地址
 *
 * $totalNum = $data["totalNum"]; //围观人数
 *
 *
