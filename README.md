 *	��Ϭֱ��PHP-SDK, �ٷ�API����
 *  @author  holger <whjsjq@gmail.com>
 *  @link
 *  @version 1.0

 * �ֶ�����
 * require_once('/path/to/Yunxizhibo-php/Yunxizhibo.php');

 *  usage:
 *   $accessKey = 'accessKey';  //��д�����õ�AccessKey
 *   $secretKey = 'secretKey';  //��д�����õ�SecretKey
 *	 $yxObj = new Yunxizhibo($accessKey, $secretKey);
 *
 *   //��ȡ��б�
 *   $data = $yxObj->getActivityList();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $list = $data["activitys"];  //�б�
 *
 *  $pageCount = $data["pageCount"]; //ҳ��
 *
 *   //��ȡ�����
 *   $data = $yxObj->getActivityInfo();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $activity = $data["activity"]; //�����
 *
 *
 *
 *   //��ȡֱ����Ƶ����
 *   $data = $yxObj->getLivestreamInfo();
 *
 *  if(empty($data)) {
 *     echo $yxObj->$errCode;
 *     echo $yxObj->$errMsg;
 *  }
 *
 *  $livestream = $data["livestream"];  //ֱ����Ƶ����
 *
 *  $wechatPlayUrl = $data["wechatPlayUrl"]; //΢��Ƕ���ַ
 *
 *  $webPlayUrl = $data["webPlayUrl"]; //��ҳǶ���ַ
 *
 *  $appPlayUrl = $data["appPlayUrl"]; //appǶ���ַ
 *
 *  $embedPlayerUrl = $data["embedPlayerUrl"]; //������Ƕ���ַ
 *
 * $totalNum = $data["totalNum"]; //Χ������
 *
 *
