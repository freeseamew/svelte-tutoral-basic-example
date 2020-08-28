<script>
	let todos = [
		{
		    id:0,
		    content: '첫 번째 할일',
		    done: false
		  },
		  {
		    id:1,
		    content: '두 번째 할일',
		    done: false
		  },
		  {
		    id:2,
		    content: '세 번째 할일',
		    done: true
		  },
		  {
		    id:3,
		    content: '네 번째 할일',
		    done: false
		  }
	]
<script>
<ul>
	{#each todos as {id, content, done}, index }
		<li>
			<span>{index + 1}</span>
			<span>{content}</span>
			<span>{done}</span>
		</li>
	{/each}
</ul>