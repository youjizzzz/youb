### [👉👉👉♥♥点此进入♥观看入口👈👈👈](http://a.d44k.cc/app.html)
<br></br><br></br><br></br>
def generate_story(data):
    """根据用户输入生成故事"""
    character = data['character']
    setting = data['setting']
    conflict = data['conflict']
    companion = data['companion']
    
    story_templates = [
        f"""
        在遥远的{setting['time']}，有一个{setting['place']}。
        那里住着一位{character['trait']}{character['profession']}，名叫{character['name']}。
        
        一天，{character['name']}得知了一个惊人的消息：{conflict}！
        为了完成这个使命，{character['name']}踏上了冒险之旅。
        
        在旅途中，{character['name']}遇到了{companion['trait']}{companion['name']}。
        他们一起克服了重重困难，最终...
        """,
        
        f"""
        {setting['time']}的{setting['place']}里，
        {character['trait']}{character['profession']} {character['name']}过着平静的生活。
        
        直到有一天，{conflict}的任务落在了{character['name']}肩上。
        虽然一开始有些害怕，但{character['name']}还是决定接受挑战。
        
        {companion['trait']}{companion['name']}自告奋勇加入冒险，
        他们的友谊在危险中不断加深，共同书写了一段传奇...
        """,
        
        f"""
        这是一个关于{character['trait']}{character['profession']} {character['name']}的故事。
        故事发生在{setting['time']}的{setting['place']}。
        
        当{conflict}的危机降临，
        {character['name']}必须挺身而出。
        
        在{companion['trait']}{companion['name']}的帮助下，
        他们展开了一场惊心动魄的冒险...
        """
    ]
    
    return random.choice(story_templates)

def main():
    """主程序流程"""
    print("📚 故事生成器 📚")
    print("----------------")
    
    user_data = get_user_input()
    story = generate_story(user_data)
    
    print("\n🎉 您的专属故事 🎉")
    print("------------------")
    print(story)
    
    print("\n感谢您的使用！")

if __name__ == "__main__":
    main()
