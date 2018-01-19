## OPERATION_STATISTICS

<pre><code>
IPHONE定义:
//资源类别
typedef enum
{
    OperationLog_CATEGORY_UnDefined = -1,//有效，但未定义
    OperationLog_CATEGORY_Invalid = 0, //无效
    OperationLog_CATEGORY_Sheet = 1 ,//歌单
    OperationLog_CATEGORY_Music = 2 ,//单曲
    OperationLog_CATEGORY_SpecialColumn = 3,//专栏
    OperationLog_CATEGORY_Album = 4 ,//专辑
    OperationLog_CATEGORY_MV = 5 ,
    OperationLog_CATEGORY_Radio = 6 ,//电台
    OperationLog_CATEGORY_Artist = 7 ,//歌手
    OperationLog_CATEGORY_Tag = 8 ,//标签
    OperationLog_CATEGORY_Area = 9 ,//专区
    OperationLog_CATEGORY_Rank = 10 ,//排行榜
    OperationLog_CATEGORY_DiscoverSong = 12 ,//发现好歌
    OperationLog_CATEGORY_More = 13 ,//更多
    OperationLog_CATEGORY_Navigation = 14 ,//导航
    OperationLog_CATEGORY_SubCategory_Tag = 15, //标签(点击后，进入的是歌单列表页面)
    
}OperationLog_CATEGORY;

//行为
typedef enum
{
    OperationLog_BEHAVIOR_Invalid,
    OperationLog_BEHAVIOR_Click,//点击
    OperationLog_BEHAVIOR_Collect, //收藏
    OperationLog_BEHAVIOR_Fav,// 红心
     OperationLog_BEHAVIOR_DesFav,// 取消红心
    OperationLog_BEHAVIOR_Share,//分享
    OperationLog_BEHAVIOR_Comment,//评论
    OperationLog_BEHAVIOR_ClickPlay,//播放  指点击行为
    OperationLog_BEHAVIOR_Download,//下载
}OperationLog_BEHAVIOR;

安卓定义：
    /**
     * RES_BEHAVIOR:资源行为。包含:
     * CLICK(点击)
     * COLLECT(收藏)
     * PLAY(播放)
     * DOWNLOAD(下载)
     * SHARE(分享)
     * LIKE(喜欢)
     * COMMENT(评论)
     * PLAY_AL(全部播放)
     * SELECT_ALL(多选)
     * ADD_TO(添加到)
     * SIMILAR(相似推荐)
     * SONG_ALBUM(查看专辑)
     * SONG_SINGER(查看歌手)
     * SONG_DETAIL(歌曲信息)
     * SET_RING(设置彩铃)
     * NEXT_PLAY(下一首播放)
     * CONCERN(关注)
     * SINGER_FANS(粉丝)
     * MINI_PLAY_PAUSE(控制栏播放暂停)
     * MINI_PLAY_NEXT(控制栏下一首)
     * MINI_CUR_LIST(控制栏播放列表)
     * SINGLE_PAY(单曲购买)
     */
    public static final String BEHAVIOR_CLICK = "CLICK";
    public static final String BEHAVIOR_COLLECT = "COLLECT";
    public static final String BEHAVIOR_SHARE = "SHARE";
    public static final String BEHAVIOR_COMMENT = "COMMENT";
    public static final String BEHAVIOR_PLAY = "PLAY";
    public static final String BEHAVIOR_DOWNLOAD = "DOWNLOAD";
    public static final String BEHAVIOR_PLAY_ALL = "PLAY_ALL";
    public static final String BEHAVIOR_SELECT_ALL = "SELECT_ALL";
    public static final String BEHAVIOR_ADD_TO = "ADD_TO";
    public static final String BEHAVIOR_SIMILAR = "SIMILAR";
    public static final String BEHAVIOR_SONG_ALBUM = "SONG_ALBUM";
    public static final String BEHAVIOR_SONG_SINGER = "SONG_SINGER";
    public static final String BEHAVIOR_LIKE = "LIKE";
    public static final String BEHAVIOR_SONG_DETAIL = "SONG_DETAIL";
    public static final String BEHAVIOR_SET_RING = "SET_RING";
    public static final String BEHAVIOR_NEXT_PLAY = "NEXT_PLAY";
    public static final String BEHAVIOR_CONCERN = "CONCERN";
    public static final String BEHAVIOR_SINGER_FANS = "SINGER_FANS";
    public static final String BEHAVIOR_MV = "MV";
    public static final String BEHAVIOR_NO_LIKE = "NO_LIKE";
    public static final String BEHAVIOR_KSONG = "KSONG";
    public static final String BEHAVIOR_MINI_PLAY_PAUSE = "MINI_PLAY_PAUSE";
    public static final String BEHAVIOR_MINI_PLAY_NEXT = "MINI_PLAY_NEXT";
    public static final String BEHAVIOR_MINI_CUR_LIST = "MINI_CUR_LIST ";
    public static final String BEHAVIOR_SHOW = "SHOW";
    public static final String BEHAVIOR_SHOW_MUSIC = "SHOW_MUSIC";
    public static final String BEHAVIOR_ADDTOLIST = "ADDTOLIST";
    public static final String BEHAVIOR_SINGLE_PAY = "SINGLE_PAY";

    /**
     * RES_CATEGORY:资源类别。包含:
     * 1(歌单);2(单曲);3(专栏);4(专辑);5(MV);6(电台);
     * 7(歌手);8(标签);9(专区);10(排行榜);11(私人口味);
     * 12(发现好歌);13(标题栏);14(导航标签);15(内链);16(列表);
     * 17(外链);18(秀场大厅);19(秀场列表);20(秀场房间);
     * 21(游戏原生页);22(H5游戏);23(侧边栏)24(我的);25(控制栏)
     * 26(煲机服务)27(老带新)28(早教)127(音效)29（云盘）30(桌面歌词)
     */
    public static final int CATEGORY_SONG_LIST = 1;
    public static final int CATEGORY_SINGLE = 2;
    public static final int CATEGORY_COLUMN = 3;
    public static final int CATEGORY_ALBUM = 4;
    public static final int CATEGORY_MV = 5;
    public static final int CATEGORY_RADIO = 6;
    public static final int CATEGORY_ARTIST = 7;
    public static final int CATEGORY_LABEL = 8;
    public static final int CATEGORY_AREA = 9;
    public static final int CATEGORY_RANKING_LIST = 10;
    public static final int CATEGORY_PRIVATE_TASTE = 11;
    public static final int CATEGORY_FOUND_SONG = 12;
    public static final int CATEGORY_TITLE_MORE = 13;
    public static final int CATEGORY_NAVIGATION = 14;
    public static final int CATEGORY_INNERLINKS = 15;
    public static final int CATEGORY_LIST = 16;
    public static final int CATEGORY_OUTERLINKS = 17;
    public static final int CATEGORY_SHOW_HALL = 18;
    public static final int CATEGORY_SHOW_LIST = 19;
    public static final int CATEGORY_SHOW_ROOM = 20;
    public static final int CATEGORY_GAME_LOCAL = 21;
    public static final int CATEGORY_GAME_H5 = 22;
    public static final int CATEGORY_SIDE_BAR = 23;
    public static final int CATEGORY_MINE = 24;
    public static final int CATEGORY_MINI_CONTROLLER = 25;
    public static final int CATEGORY_BURN = 26;
    public static final int CATEGORY_BIND_NEW = 27;
    public static final int CATEGORY_CHILD = 28;
    public static final int CATEGORY_YUNPAN = 29; //云盘相关
    public static final int CATEGORY_DESK_LYRIC = 30;
    public static final int CATEGORY_FEED_BIBI = 123;
    public static final int CATEGORY_FEED_PGC = 124;
    public static final int CATEGORY_FEED_RECOMMEND = 125;
    public static final int CATEGORY_EXT_MV = 126;
    public static final int CATEGORY_AUDIO_EFFECT = 127;
</code></pre>
